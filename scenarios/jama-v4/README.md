# JAMA SAKURA V4.0 Scenario Framework

Based on JAMA (Japan Automobile Manufacturers Association) SAKURA Project V4.0, 344 pages, 7 Annexes (A-G).

## Framework Overview

### Three Disturbance Categories

| ID | Category | DDT Process | Physical Basis |
|---|---|---|---|
| D-1 | Perception Disturbance (感知干扰) | Perception | Sensor physics: radar EM, LiDAR IR, camera visible light |
| D-2 | Traffic Disturbance (交通干扰) | Decision | Road geometry x ego behavior x surrounding vehicle combinations |
| D-3 | Vehicle Dynamics Disturbance (车辆动力学干扰) | Operation | Road surface, weather, tire state |

### Four-Quadrant Safety Model (UN/WP29)

| Quadrant | Foreseeable | Preventable | Description |
|---|---|---|---|
| A | Yes | Yes | ADS must avoid — primary evaluation target |
| B | Yes | No | Beyond capability even for competent human |
| C | No | Yes | Unforeseeable but technically avoidable |
| D | No | No | Unforeseeable and unavoidable |

### Scenario Abstraction (3 Layers)

| Layer | Description |
|---|---|
| Functional Scenario (功能场景) | Qualitative description |
| Logical Scenario (逻辑场景) | Parameterized with ranges |
| Concrete Scenario (具体场景) | Specific values for test execution |

## Key Numbers

- **58** traffic disturbance scenario types
- **32** theoretical multi-vehicle spatial patterns (Annex C)
- **5-8** commonly occurring patterns (data-driven, 80/20 rule)
- **3** preventability boundary scenarios (Cut-in, Cut-out, Deceleration)
- **3** accident databases validated (GIDAS 90%, ITARDA 99.89%)

## C&C Driver Model Parameters

| Parameter | Value | Source |
|---|---|---|
| Perception-to-deceleration delay | 0.75s | Japanese NPA standard |
| Maximum deceleration | 0.774G | Makishita et al. (2001) |
| Time to reach max deceleration | ~0.6s | Braking waveform analysis |
