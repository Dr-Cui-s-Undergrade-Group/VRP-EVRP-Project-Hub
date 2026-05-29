# Benchmarks and Metrics

## 1. Problem Variants

| Variant | Description | 中文说明 |
|---|---|---|
| CVRP | capacitated vehicle routing problem | 容量约束车辆路径问题 |
| VRPTW | VRP with customer time windows | 带客户时间窗的车辆路径问题 |
| EVRP-TW | electric vehicle routing with time windows, battery limits, and recharging | 考虑电量、充电站和时间窗的电动车路径问题 |
| Truck-drone routing | coordinated ground-air delivery with launch, recovery, and synchronization | 卡车与无人机协同配送，需要考虑发射、回收和同步 |
| Ground-air collaborative EVRP-TW | truck-drone routing plus battery, time-window, and charging constraints | 在空地协同基础上加入电量、时间窗和充电约束 |

## 2. Core Metrics

| Metric | Use for | 中文说明 |
|---|---|---|
| Total distance / cost | all variants | 总路程或总成本 |
| Feasibility rate | all variants | 可行解比例 |
| Runtime | all variants | 求解时间 |
| Time-window violations | VRPTW, EVRP-TW, truck-drone | 时间窗违约次数或惩罚 |
| Capacity violations | CVRP and extensions | 容量违约 |
| Energy violations | EVRP-TW | 电量不足或充电约束违约 |
| Charging count / charging time | EVRP-TW | 充电次数与充电时间 |
| Makespan | truck-drone collaboration | 完工时间，尤其适合协同配送 |
| Synchronization violations | truck-drone collaboration | 无人机与卡车等待、错过回收点等同步问题 |

## 3. Minimum Reporting Standard

Each team should report:

1. Baseline and improved method on at least 3 instance sizes or 3 representative instances.
2. Objective value and feasibility together.
3. Runtime and hardware.
4. Random seeds and solver parameters.
5. At least 3 failure cases with constraint-level diagnosis.

中文最低要求：

每组至少在 3 种规模或 3 个代表性算例上比较基线与改进方法，同时报告目标值、可行性、运行时间、硬件、随机种子和求解器参数。不能只报告“最短距离”。

## 4. Failure Analysis Template

For each failed or poor route, record:

- instance name and size;
- solver or model;
- objective value;
- feasibility status;
- violated constraints;
- where the route first becomes infeasible;
- possible fix or next experiment.

中文模板：

- 算例名称与规模；
- 使用的求解器或模型；
- 目标值；
- 是否可行；
- 违反了哪些约束；
- 路径在哪一步开始不可行；
- 下一步如何修复或验证。

## 5. Recommended Baseline Ladder

1. CVRP with OR-Tools or PyVRP.
2. VRPTW with explicit time-window reporting.
3. EVRP-TW with battery and charging checks.
4. Neural construction baseline such as POMO.
5. Hybrid method or truck-drone extension.

This ladder keeps the project reproducible. If Step 2 does not run, Step 5 will not be meaningful.
