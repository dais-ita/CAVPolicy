# Connected and Autonomous Vehicle Annotated Policies

This repository contains the dataset and [Controlled English (CE)](https://github.com/ce-store/ce-store) model used in the publication *"An Answer Set Grammar-based Generative Policy Model for Connected and Autonomous Vehicles"*.

## Dataset

### Format
|driving_task_type|control|monitoring|fallback|weather|visibility|traffic_congestion|environmental_weighted_average|driving_task_loa|vehicle_loa|region_loa|result
|---|---|---|---|---|---|---|---|---|---|---|---|
|adaptive speed control|human and system|human|human|0|0|0|0|1|3|4|approved|

### Explanation
[cav_policies.csv](cav_policies.csv) contains 239,580 annotated policies for Connected and Autonomous Vehicles (CAVs) generated using the CE model [outlined below](#ce-model). The dataset is based around the [SAE Levels of Autonomy (LoA)](https://www.sae.org/standards/content/j3016_201806/), where each row represents a vehicle located in a particular region attempting to execute a driving task under certain environmental conditions. The details of the particular driving task align with the SAE Levels of Autonomy in terms of who is responsible for controlling the vehicle, monitoring the driving environment and who holds fallback responsibility for the driving task. The environmental conditions (`weather`, `visibility` and `traffic congestion`) contain integer values between 0 and 10 inclusive, to represent the severity of the condition and are combined into a weighted average score using the weights listed in [environmental_weights.csv](environmental_weights.csv). The Level of Autonomy (LoA) of the vehicle and the LoA permitted in each region is given and the result indicates whether this particular policy is `approved` or `rejected` according to the LoA of the vehicle, region and driving task. To decide the `approve/reject` annotation, we first impose thresholds to evaluate the LoA of the requested driving task, which is executed under certain environmental conditions outlined in each policy. If the environmental conditions score is >= 95, the driving task is level 5 always and to distinguish between level 4 and level 5 driving tasks, a score of >= 75 is required, provided also the system is responsible for controlling the vehicle, monitoring the driving environment and has fallback responsibility of the driving task. Finally, a policy should be `approved` iff Vehicle LoA >= Task LoA <= Region LoA otherwise the policy should be `rejected`. We instantiate the CE model below with 6 vehicles, 6 regions and 5 driving tasks, where each vehicle, region and driving task correspond to a different LoA. Note that only 5 driving tasks are specified as the only difference between a level 4 task and a level 5 task is the environmental conditions under which it is executed. It is possible to distinguish between levels 0-3 inclusive by evaluating who is responsible for controlling the vehicle, monitoring the driving environment and who holds ultimate responsibility for the driving task. Also, the SAE standard specification states that at levels 0-4 inclusive, there are some extreme driving modes that a vehicle may not be able to operate autonomously under and therefore if a user requests to execute a driving task rated at levels 0-4 inclusive, it may require level 5 automation from the vehicle under these extreme conditions. Given 6 vehicles, 6 regions, 5 tasks and 1331 = 3^11 possible environmental conditions, 239580= 6 * 6 * 5 * 1331 annotated policies are created.


## CE Model
We utilise CE to provide a semantic knowledge base for the CAV domain, which enables us to generate the dataset described above. The [ce](ce) folder contains the code explained in this section. The LOA concept can be modelled with a CE statement as shown below, where LOA is a concept in our domain model named `level of autonomy`. The `level of autonomy` concept includes values such as the `SAE Level` (i.e., an integer value between 0 and 5), a `definition` (i.e., *level 2 provides one or more driver assistance functions*), an indication as to who is `responsible for vehicle control`  (e.g., the system), who is `responsible for monitoring
the driving environment` (e.g., a human), and who is `ultimately responsible for the dynamic driving task` (e.g. a human).   
 
```
conceptualise a ~ level of autonomy ~ LOA that
  has the value SAE as ~ SAE Level ~ and
  has the value DEF as ~ definition ~ and
  has the value X as ~ responsible for vehicle control ~ and 
  has the value M as ~ responsible for monitoring the driving environment ~ and 
  has the value F as ~ ultimately responsible for the dynamic driving task ~. 
```

To instantiate the LOA concept, we use the CE statement shown below, which states that there is an instance named `conditional automation` of the `level of autonomy` concept that has `SAE Level` 3 and a `definition`: *The driving mode-specific performance by an automated driving system of all aspects of the dynamic driving task with the expectation that the human driver will respond appropriately to a request to intervene.* At this LOA the CAV is both responsible for vehicle control and for monitoring the driving environment but ultimately a human is responsible for the dynamic driving task.
```
there is a level of autonomy named 'conditional 
automation' that
  has the value '3' as SAE Level and
  has the value 'The driving mode-specific performance by an automated driving system of all aspects of the dynamic driving task with the expectation that the human driver will respond appropriately to a request to intervene.' as definition and
  has the value 'system' as responsible for vehicle control and 
  has the value 'system' as responsible for monitoring the driving environment and
  has the value 'human' as ultimately responsible for the dynamic driving task.
```

The CE model also includes the concepts of driving tasks, driving task instances, vehicles, regions and environmental conditions. These are shown below and can be described as follows:
1. There is a concept named `driving task` that has a `description` (e.g. *Turning the vehicle left or right at a given junction. The human driver may have to intervene at blind corners.*) along with values as to which entity is responsible for vehicle control (e.g. the system), monitoring the driving environment (e.g. the system) and who is ultimately responsible for the driving task (e.g. a human).
2. There is a concept named `driving task instance` that is an instance of a `driving task` and is executed in a set of environmental conditions (e.g. good visibility, sunny weather, low traffic congestion) and therefore requires a minimum SAE LOA (e.g. 3).
3. There is a concept named `region` that has a `GeoJSON polygon` as an area value. The region `permits` a particular SAE LOA (e.g. 4).  
4. There is a concept named `vehicle` that has a `GeoJSON point` as a value to denote the current location which is `located within` a specific region. The vehicle `is capable of operating at` a defined SAE LOA (e.g. 4).
5. There is a concept named `roadside unit` which is located at a `GeoJSON point` and `is located within` a region.
6. Environmental conditions such as `visibility level`, `weather condition` and `traffic congestion level` concepts are also modelled, to define the visibility, weather type and severity respectively.

```
conceptualise a ~ driving task ~ DT that
  has the value DESC as ~ description ~ and
  has the value C as ~ responsible for vehicle control ~ and
  has the value M as ~ responsible for monitoring the driving environment ~ and
  has the value F as ~ ultimately responsible for the dynamic driving task ~.
  
conceptualise a ~ driving task instance ~ DTI that
  ~ is an instance of ~ the driving task DT and
  ~ is executed in ~ the environmental condition score ECS and
  ~ requires ~ the level of autonomy LOA ~.

conceptualise a ~ region ~ R that
  has the value POLY as ~ GeoJSON polygon ~ and
  ~ permits ~ the level of autonomy LOA.
  
conceptualise a ~ vehicle ~ V that
  has the value POINT as ~ GeoJSON point ~ and
  ~ is located within ~ the region R and
  ~ is capable of operating at ~ the level of autonomy LOA.

conceptualise an ~ environmental condition ~ EC that
  has the value W as ~ calculation weight ~.

conceptualise an ~ environmental condition score ~ ECS that
  ~ contains ~ the visibility level VL and
  ~ contains ~ the weather condition WC and
  ~ contains ~ the traffic congestion level TCL and
  has the value S as ~ score ~.

conceptualise a ~ visibility level ~ VL that
  is an environmental condition and
  has the value CW as ~ calculation weight ~ and
  has the value V as ~ visibility ~.

conceptualise a ~ weather condition ~ WC that
  is an environmental condition and
  has the value CW as ~ calculation weight ~ and
  has the value WT as ~ weather type ~.

conceptualise a ~ traffic congestion level ~ TCL that
  is an environmental condition and
  has the value CW as ~ calculation weight ~ and
  has the value S as ~ severity ~.
```

## Cite
If you use this code or the datasets please make sure that you cite the following papers:
> TBC
