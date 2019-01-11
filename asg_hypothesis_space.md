# Answer Set Grammar Hypothesis Space

The following is the complete Answer Set Grammar (ASG) hypothesis space of the learning task in Example 2 of the publication "An Answer Set Grammar-based Generative Policy Model for Connected and Autonomous Vehicles".

```
1:[1] ~ driving_loa(0).
1:[1] ~ driving_loa(1).
1:[1] ~ driving_loa(2).
1:[1] ~ driving_loa(3).
1:[1] ~ driving_loa(4).
1:[1] ~ driving_loa(5).
1:[1] ~ reject.
2:[1] ~ driving_loa(0) :- control("human and system")@1.
2:[1] ~ driving_loa(0) :- control("human")@1.
2:[1] ~ driving_loa(0) :- control("system")@1.
2:[1] ~ driving_loa(0) :- fallback("human")@5.
2:[1] ~ driving_loa(0) :- fallback("system")@5.
2:[1] ~ driving_loa(0) :- monitoring("human")@3.
2:[1] ~ driving_loa(0) :- monitoring("system")@3.
2:[1] ~ driving_loa(1) :- control("human and system")@1.
2:[1] ~ driving_loa(1) :- control("human")@1.
2:[1] ~ driving_loa(1) :- control("system")@1.
2:[1] ~ driving_loa(1) :- fallback("human")@5.
2:[1] ~ driving_loa(1) :- fallback("system")@5.
2:[1] ~ driving_loa(1) :- monitoring("human")@3.
2:[1] ~ driving_loa(1) :- monitoring("system")@3.
2:[1] ~ driving_loa(2) :- control("human and system")@1.
2:[1] ~ driving_loa(2) :- control("human")@1.
2:[1] ~ driving_loa(2) :- control("system")@1.
2:[1] ~ driving_loa(2) :- fallback("human")@5.
2:[1] ~ driving_loa(2) :- fallback("system")@5.
2:[1] ~ driving_loa(2) :- monitoring("human")@3.
2:[1] ~ driving_loa(2) :- monitoring("system")@3.
2:[1] ~ driving_loa(3) :- control("human and system")@1.
2:[1] ~ driving_loa(3) :- control("human")@1.
2:[1] ~ driving_loa(3) :- control("system")@1.
2:[1] ~ driving_loa(3) :- fallback("human")@5.
2:[1] ~ driving_loa(3) :- fallback("system")@5.
2:[1] ~ driving_loa(3) :- monitoring("human")@3.
2:[1] ~ driving_loa(3) :- monitoring("system")@3.
2:[1] ~ driving_loa(4) :- control("human and system")@1.
2:[1] ~ driving_loa(4) :- control("human")@1.
2:[1] ~ driving_loa(4) :- control("system")@1.
2:[1] ~ driving_loa(4) :- fallback("human")@5.
2:[1] ~ driving_loa(4) :- fallback("system")@5.
2:[1] ~ driving_loa(4) :- monitoring("human")@3.
2:[1] ~ driving_loa(4) :- monitoring("system")@3.
2:[1] ~ driving_loa(5) :- control("human and system")@1.
2:[1] ~ driving_loa(5) :- control("human")@1.
2:[1] ~ driving_loa(5) :- control("system")@1.
2:[1] ~ driving_loa(5) :- fallback("human")@5.
2:[1] ~ driving_loa(5) :- fallback("system")@5.
2:[1] ~ driving_loa(5) :- monitoring("human")@3.
2:[1] ~ driving_loa(5) :- monitoring("system")@3.
3:[1] ~ driving_loa(0) :- V0_user > 0, region_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 0, vehicle_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 1, region_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 1, vehicle_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 2, region_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 2, vehicle_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 20, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 22, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 3, region_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 3, vehicle_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 31, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 33, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 4, region_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 4, vehicle_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 48, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 5, region_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 5, vehicle_loa(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 50, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 52, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 60, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 74, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 75, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- V0_user > 79, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(0) :- fallback("human")@5, control("human and system")@1.
3:[1] ~ driving_loa(0) :- fallback("human")@5, control("human")@1.
3:[1] ~ driving_loa(0) :- fallback("human")@5, control("system")@1.
3:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("human")@3.
3:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("system")@3.
3:[1] ~ driving_loa(0) :- fallback("system")@5, control("human and system")@1.
3:[1] ~ driving_loa(0) :- fallback("system")@5, control("human")@1.
3:[1] ~ driving_loa(0) :- fallback("system")@5, control("system")@1.
3:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("human")@3.
3:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("system")@3.
3:[1] ~ driving_loa(0) :- monitoring("human")@3, control("human and system")@1.
3:[1] ~ driving_loa(0) :- monitoring("human")@3, control("human")@1.
3:[1] ~ driving_loa(0) :- monitoring("human")@3, control("system")@1.
3:[1] ~ driving_loa(0) :- monitoring("system")@3, control("human and system")@1.
3:[1] ~ driving_loa(0) :- monitoring("system")@3, control("human")@1.
3:[1] ~ driving_loa(0) :- monitoring("system")@3, control("system")@1.
3:[1] ~ driving_loa(0) :- region_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(0) :- region_loa(V0_user), vehicle_loa(V0_user).
3:[1] ~ driving_loa(0) :- vehicle_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 0, region_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 0, vehicle_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 1, region_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 1, vehicle_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 2, region_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 2, vehicle_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 20, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 22, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 3, region_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 3, vehicle_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 31, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 33, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 4, region_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 4, vehicle_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 48, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 5, region_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 5, vehicle_loa(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 50, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 52, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 60, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 74, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 75, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- V0_user > 79, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(1) :- fallback("human")@5, control("human and system")@1.
3:[1] ~ driving_loa(1) :- fallback("human")@5, control("human")@1.
3:[1] ~ driving_loa(1) :- fallback("human")@5, control("system")@1.
3:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("human")@3.
3:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("system")@3.
3:[1] ~ driving_loa(1) :- fallback("system")@5, control("human and system")@1.
3:[1] ~ driving_loa(1) :- fallback("system")@5, control("human")@1.
3:[1] ~ driving_loa(1) :- fallback("system")@5, control("system")@1.
3:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("human")@3.
3:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("system")@3.
3:[1] ~ driving_loa(1) :- monitoring("human")@3, control("human and system")@1.
3:[1] ~ driving_loa(1) :- monitoring("human")@3, control("human")@1.
3:[1] ~ driving_loa(1) :- monitoring("human")@3, control("system")@1.
3:[1] ~ driving_loa(1) :- monitoring("system")@3, control("human and system")@1.
3:[1] ~ driving_loa(1) :- monitoring("system")@3, control("human")@1.
3:[1] ~ driving_loa(1) :- monitoring("system")@3, control("system")@1.
3:[1] ~ driving_loa(1) :- region_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(1) :- region_loa(V0_user), vehicle_loa(V0_user).
3:[1] ~ driving_loa(1) :- vehicle_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 0, region_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 0, vehicle_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 1, region_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 1, vehicle_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 2, region_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 2, vehicle_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 20, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 22, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 3, region_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 3, vehicle_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 31, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 33, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 4, region_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 4, vehicle_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 48, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 5, region_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 5, vehicle_loa(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 50, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 52, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 60, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 74, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 75, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- V0_user > 79, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(2) :- fallback("human")@5, control("human and system")@1.
3:[1] ~ driving_loa(2) :- fallback("human")@5, control("human")@1.
3:[1] ~ driving_loa(2) :- fallback("human")@5, control("system")@1.
3:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("human")@3.
3:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("system")@3.
3:[1] ~ driving_loa(2) :- fallback("system")@5, control("human and system")@1.
3:[1] ~ driving_loa(2) :- fallback("system")@5, control("human")@1.
3:[1] ~ driving_loa(2) :- fallback("system")@5, control("system")@1.
3:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("human")@3.
3:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("system")@3.
3:[1] ~ driving_loa(2) :- monitoring("human")@3, control("human and system")@1.
3:[1] ~ driving_loa(2) :- monitoring("human")@3, control("human")@1.
3:[1] ~ driving_loa(2) :- monitoring("human")@3, control("system")@1.
3:[1] ~ driving_loa(2) :- monitoring("system")@3, control("human and system")@1.
3:[1] ~ driving_loa(2) :- monitoring("system")@3, control("human")@1.
3:[1] ~ driving_loa(2) :- monitoring("system")@3, control("system")@1.
3:[1] ~ driving_loa(2) :- region_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(2) :- region_loa(V0_user), vehicle_loa(V0_user).
3:[1] ~ driving_loa(2) :- vehicle_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 0, region_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 0, vehicle_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 1, region_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 1, vehicle_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 2, region_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 2, vehicle_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 20, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 22, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 3, region_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 3, vehicle_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 31, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 33, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 4, region_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 4, vehicle_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 48, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 5, region_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 5, vehicle_loa(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 50, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 52, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 60, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 74, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 75, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- V0_user > 79, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(3) :- fallback("human")@5, control("human and system")@1.
3:[1] ~ driving_loa(3) :- fallback("human")@5, control("human")@1.
3:[1] ~ driving_loa(3) :- fallback("human")@5, control("system")@1.
3:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("human")@3.
3:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("system")@3.
3:[1] ~ driving_loa(3) :- fallback("system")@5, control("human and system")@1.
3:[1] ~ driving_loa(3) :- fallback("system")@5, control("human")@1.
3:[1] ~ driving_loa(3) :- fallback("system")@5, control("system")@1.
3:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("human")@3.
3:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("system")@3.
3:[1] ~ driving_loa(3) :- monitoring("human")@3, control("human and system")@1.
3:[1] ~ driving_loa(3) :- monitoring("human")@3, control("human")@1.
3:[1] ~ driving_loa(3) :- monitoring("human")@3, control("system")@1.
3:[1] ~ driving_loa(3) :- monitoring("system")@3, control("human and system")@1.
3:[1] ~ driving_loa(3) :- monitoring("system")@3, control("human")@1.
3:[1] ~ driving_loa(3) :- monitoring("system")@3, control("system")@1.
3:[1] ~ driving_loa(3) :- region_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(3) :- region_loa(V0_user), vehicle_loa(V0_user).
3:[1] ~ driving_loa(3) :- vehicle_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 0, region_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 0, vehicle_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 1, region_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 1, vehicle_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 2, region_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 2, vehicle_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 20, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 22, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 3, region_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 3, vehicle_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 31, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 33, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 4, region_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 4, vehicle_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 48, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 5, region_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 5, vehicle_loa(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 50, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 52, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 60, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 74, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 75, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- V0_user > 79, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(4) :- fallback("human")@5, control("human and system")@1.
3:[1] ~ driving_loa(4) :- fallback("human")@5, control("human")@1.
3:[1] ~ driving_loa(4) :- fallback("human")@5, control("system")@1.
3:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("human")@3.
3:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("system")@3.
3:[1] ~ driving_loa(4) :- fallback("system")@5, control("human and system")@1.
3:[1] ~ driving_loa(4) :- fallback("system")@5, control("human")@1.
3:[1] ~ driving_loa(4) :- fallback("system")@5, control("system")@1.
3:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("human")@3.
3:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("system")@3.
3:[1] ~ driving_loa(4) :- monitoring("human")@3, control("human and system")@1.
3:[1] ~ driving_loa(4) :- monitoring("human")@3, control("human")@1.
3:[1] ~ driving_loa(4) :- monitoring("human")@3, control("system")@1.
3:[1] ~ driving_loa(4) :- monitoring("system")@3, control("human and system")@1.
3:[1] ~ driving_loa(4) :- monitoring("system")@3, control("human")@1.
3:[1] ~ driving_loa(4) :- monitoring("system")@3, control("system")@1.
3:[1] ~ driving_loa(4) :- region_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(4) :- region_loa(V0_user), vehicle_loa(V0_user).
3:[1] ~ driving_loa(4) :- vehicle_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 0, region_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 0, vehicle_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 1, region_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 1, vehicle_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 2, region_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 2, vehicle_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 20, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 22, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 3, region_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 3, vehicle_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 31, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 33, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 4, region_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 4, vehicle_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 48, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 5, region_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 5, vehicle_loa(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 50, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 52, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 60, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 74, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 75, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- V0_user > 79, weighted_avg_dynamic_features(V0_user).
3:[1] ~ driving_loa(5) :- fallback("human")@5, control("human and system")@1.
3:[1] ~ driving_loa(5) :- fallback("human")@5, control("human")@1.
3:[1] ~ driving_loa(5) :- fallback("human")@5, control("system")@1.
3:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("human")@3.
3:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("system")@3.
3:[1] ~ driving_loa(5) :- fallback("system")@5, control("human and system")@1.
3:[1] ~ driving_loa(5) :- fallback("system")@5, control("human")@1.
3:[1] ~ driving_loa(5) :- fallback("system")@5, control("system")@1.
3:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("human")@3.
3:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("system")@3.
3:[1] ~ driving_loa(5) :- monitoring("human")@3, control("human and system")@1.
3:[1] ~ driving_loa(5) :- monitoring("human")@3, control("human")@1.
3:[1] ~ driving_loa(5) :- monitoring("human")@3, control("system")@1.
3:[1] ~ driving_loa(5) :- monitoring("system")@3, control("human and system")@1.
3:[1] ~ driving_loa(5) :- monitoring("system")@3, control("human")@1.
3:[1] ~ driving_loa(5) :- monitoring("system")@3, control("system")@1.
3:[1] ~ driving_loa(5) :- region_loa(V0_user), driving_loa(V0_user).
3:[1] ~ driving_loa(5) :- region_loa(V0_user), vehicle_loa(V0_user).
3:[1] ~ driving_loa(5) :- vehicle_loa(V0_user), driving_loa(V0_user).
3:[1] ~ reject :- V0_user > 0, region_loa(V0_user).
3:[1] ~ reject :- V0_user > 0, vehicle_loa(V0_user).
3:[1] ~ reject :- V0_user > 1, region_loa(V0_user).
3:[1] ~ reject :- V0_user > 1, vehicle_loa(V0_user).
3:[1] ~ reject :- V0_user > 2, region_loa(V0_user).
3:[1] ~ reject :- V0_user > 2, vehicle_loa(V0_user).
3:[1] ~ reject :- V0_user > 20, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 22, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 3, region_loa(V0_user).
3:[1] ~ reject :- V0_user > 3, vehicle_loa(V0_user).
3:[1] ~ reject :- V0_user > 31, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 33, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 4, region_loa(V0_user).
3:[1] ~ reject :- V0_user > 4, vehicle_loa(V0_user).
3:[1] ~ reject :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 40, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 48, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 5, region_loa(V0_user).
3:[1] ~ reject :- V0_user > 5, vehicle_loa(V0_user).
3:[1] ~ reject :- V0_user > 50, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 52, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 60, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 72, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 74, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 75, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- V0_user > 79, weighted_avg_dynamic_features(V0_user).
3:[1] ~ reject :- region_loa(V0_user), driving_loa(V0_user).
3:[1] ~ reject :- region_loa(V0_user), vehicle_loa(V0_user).
3:[1] ~ reject :- vehicle_loa(V0_user), driving_loa(V0_user).
4:[1] ~ driving_loa(0) :- V0_user < V1_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(0) :- V0_user < V2_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(0) :- V0_user < V2_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(0) :- V1_user < V0_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(0) :- V1_user > 0, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 0, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 0, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 0, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 0, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 0, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 0, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 0, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 0, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 0, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 0, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 0, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 0, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 0, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 1, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 1, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 1, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 1, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 1, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 1, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 1, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 1, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 1, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 1, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 1, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 1, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 1, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 1, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 2, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 2, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 2, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 2, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 2, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 2, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 2, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 2, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 2, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 2, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 2, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 2, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 2, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 2, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 3, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 3, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 3, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 3, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 3, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 3, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 3, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 3, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 3, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 3, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 3, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 3, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 3, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 3, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 4, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 4, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 4, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 4, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 4, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 4, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 4, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 4, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 4, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 4, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 4, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 4, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 4, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 4, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 5, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 5, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 5, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 5, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 5, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 5, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 5, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 5, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 5, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 5, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 5, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 5, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 5, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 5, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- V2_user < V0_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(0) :- V2_user < V0_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(0) :- fallback("human")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(0) :- fallback("system")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(0) :- region_loa(V0_user), vehicle_loa(V0_user), driving_loa(V0_user).
4:[1] ~ driving_loa(0) :- region_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(0) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(0) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(0) :- vehicle_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(0) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(0) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(0) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(0) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V0_user < V1_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(1) :- V0_user < V2_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(1) :- V0_user < V2_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(1) :- V1_user < V0_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(1) :- V1_user > 0, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 0, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 0, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 0, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 0, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 0, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 0, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 0, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 0, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 0, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 0, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 0, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 0, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 0, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 1, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 1, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 1, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 1, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 1, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 1, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 1, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 1, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 1, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 1, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 1, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 1, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 1, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 1, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 2, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 2, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 2, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 2, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 2, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 2, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 2, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 2, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 2, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 2, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 2, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 2, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 2, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 2, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 3, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 3, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 3, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 3, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 3, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 3, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 3, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 3, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 3, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 3, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 3, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 3, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 3, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 3, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 4, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 4, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 4, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 4, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 4, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 4, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 4, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 4, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 4, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 4, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 4, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 4, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 4, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 4, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 5, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 5, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 5, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 5, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 5, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 5, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 5, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 5, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 5, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 5, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 5, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 5, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 5, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 5, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- V2_user < V0_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(1) :- V2_user < V0_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(1) :- fallback("human")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(1) :- fallback("system")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(1) :- region_loa(V0_user), vehicle_loa(V0_user), driving_loa(V0_user).
4:[1] ~ driving_loa(1) :- region_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(1) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(1) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(1) :- vehicle_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(1) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(1) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(1) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(1) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V0_user < V1_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(2) :- V0_user < V2_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(2) :- V0_user < V2_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(2) :- V1_user < V0_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(2) :- V1_user > 0, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 0, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 0, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 0, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 0, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 0, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 0, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 0, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 0, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 0, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 0, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 0, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 0, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 0, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 1, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 1, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 1, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 1, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 1, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 1, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 1, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 1, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 1, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 1, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 1, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 1, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 1, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 1, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 2, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 2, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 2, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 2, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 2, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 2, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 2, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 2, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 2, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 2, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 2, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 2, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 2, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 2, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 3, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 3, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 3, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 3, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 3, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 3, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 3, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 3, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 3, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 3, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 3, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 3, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 3, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 3, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 4, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 4, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 4, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 4, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 4, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 4, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 4, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 4, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 4, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 4, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 4, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 4, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 4, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 4, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 5, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 5, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 5, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 5, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 5, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 5, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 5, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 5, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 5, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 5, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 5, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 5, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 5, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 5, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- V2_user < V0_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(2) :- V2_user < V0_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(2) :- fallback("human")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(2) :- fallback("system")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(2) :- region_loa(V0_user), vehicle_loa(V0_user), driving_loa(V0_user).
4:[1] ~ driving_loa(2) :- region_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(2) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(2) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(2) :- vehicle_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(2) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(2) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(2) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(2) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V0_user < V1_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(3) :- V0_user < V2_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(3) :- V0_user < V2_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(3) :- V1_user < V0_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(3) :- V1_user > 0, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 0, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 0, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 0, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 0, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 0, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 0, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 0, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 0, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 0, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 0, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 0, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 0, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 0, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 1, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 1, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 1, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 1, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 1, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 1, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 1, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 1, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 1, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 1, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 1, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 1, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 1, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 1, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 2, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 2, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 2, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 2, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 2, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 2, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 2, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 2, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 2, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 2, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 2, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 2, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 2, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 2, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 3, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 3, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 3, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 3, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 3, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 3, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 3, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 3, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 3, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 3, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 3, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 3, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 3, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 3, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 4, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 4, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 4, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 4, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 4, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 4, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 4, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 4, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 4, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 4, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 4, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 4, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 4, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 4, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 5, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 5, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 5, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 5, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 5, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 5, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 5, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 5, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 5, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 5, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 5, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 5, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 5, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 5, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- V2_user < V0_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(3) :- V2_user < V0_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(3) :- fallback("human")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(3) :- fallback("system")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(3) :- region_loa(V0_user), vehicle_loa(V0_user), driving_loa(V0_user).
4:[1] ~ driving_loa(3) :- region_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(3) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(3) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(3) :- vehicle_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(3) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(3) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(3) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(3) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V0_user < V1_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(4) :- V0_user < V2_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(4) :- V0_user < V2_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(4) :- V1_user < V0_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(4) :- V1_user > 0, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 0, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 0, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 0, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 0, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 0, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 0, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 0, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 0, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 0, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 0, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 0, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 0, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 0, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 1, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 1, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 1, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 1, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 1, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 1, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 1, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 1, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 1, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 1, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 1, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 1, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 1, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 1, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 2, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 2, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 2, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 2, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 2, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 2, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 2, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 2, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 2, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 2, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 2, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 2, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 2, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 2, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 3, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 3, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 3, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 3, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 3, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 3, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 3, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 3, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 3, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 3, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 3, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 3, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 3, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 3, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 4, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 4, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 4, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 4, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 4, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 4, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 4, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 4, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 4, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 4, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 4, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 4, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 4, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 4, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 5, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 5, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 5, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 5, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 5, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 5, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 5, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 5, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 5, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 5, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 5, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 5, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 5, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 5, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- V2_user < V0_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(4) :- V2_user < V0_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(4) :- fallback("human")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(4) :- fallback("system")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(4) :- region_loa(V0_user), vehicle_loa(V0_user), driving_loa(V0_user).
4:[1] ~ driving_loa(4) :- region_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(4) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(4) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(4) :- vehicle_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(4) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(4) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(4) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(4) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V0_user < V1_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(5) :- V0_user < V2_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(5) :- V0_user < V2_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(5) :- V1_user < V0_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ driving_loa(5) :- V1_user > 0, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 0, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 0, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 0, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 0, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 0, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 0, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 0, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 0, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 0, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 0, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 0, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 0, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 0, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 1, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 1, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 1, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 1, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 1, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 1, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 1, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 1, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 1, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 1, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 1, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 1, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 1, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 1, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 2, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 2, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 2, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 2, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 2, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 2, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 2, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 2, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 2, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 2, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 2, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 2, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 2, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 2, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 20, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 22, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 3, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 3, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 3, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 3, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 3, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 3, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 3, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 3, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 3, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 3, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 3, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 3, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 3, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 3, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 31, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 33, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 4, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 4, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 4, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 4, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 4, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 4, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 4, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 4, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 4, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 4, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 4, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 4, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 4, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 4, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 40, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 48, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 5, region_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 5, region_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 5, region_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 5, region_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 5, region_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 5, region_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 5, region_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 5, vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 5, vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 5, vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 5, vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 5, vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 5, vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 5, vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 50, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 52, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 60, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 72, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 74, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 75, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- V1_user > 79, weighted_avg_dynamic_features(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- V2_user < V0_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(5) :- V2_user < V0_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(5) :- fallback("human")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("human")@3, control("human and system")@1.
4:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("human")@3, control("human")@1.
4:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("human")@3, control("system")@1.
4:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("system")@3, control("human and system")@1.
4:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("system")@3, control("human")@1.
4:[1] ~ driving_loa(5) :- fallback("system")@5, monitoring("system")@3, control("system")@1.
4:[1] ~ driving_loa(5) :- region_loa(V0_user), vehicle_loa(V0_user), driving_loa(V0_user).
4:[1] ~ driving_loa(5) :- region_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), vehicle_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), vehicle_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), vehicle_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), vehicle_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- region_loa(V1_user), vehicle_loa(V1_user), monitoring("system")@3.
4:[1] ~ driving_loa(5) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human and system")@1.
4:[1] ~ driving_loa(5) :- vehicle_loa(V1_user), driving_loa(V1_user), control("human")@1.
4:[1] ~ driving_loa(5) :- vehicle_loa(V1_user), driving_loa(V1_user), control("system")@1.
4:[1] ~ driving_loa(5) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("human")@5.
4:[1] ~ driving_loa(5) :- vehicle_loa(V1_user), driving_loa(V1_user), fallback("system")@5.
4:[1] ~ driving_loa(5) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("human")@3.
4:[1] ~ driving_loa(5) :- vehicle_loa(V1_user), driving_loa(V1_user), monitoring("system")@3.
4:[1] ~ reject :- V0_user < V1_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ reject :- V0_user < V2_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ reject :- V0_user < V2_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ reject :- V1_user < V0_user, region_loa(V1_user), vehicle_loa(V0_user).
4:[1] ~ reject :- V2_user < V0_user, region_loa(V2_user), driving_loa(V0_user).
4:[1] ~ reject :- V2_user < V0_user, vehicle_loa(V2_user), driving_loa(V0_user).
4:[1] ~ reject :- region_loa(V0_user), vehicle_loa(V0_user), driving_loa(V0_user).
```
