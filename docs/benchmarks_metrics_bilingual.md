# Benchmarks and Metrics | 基准与指标

## 1. Problem variants | 问题类型

### EN
- CVRP: capacity-constrained VRP.
- VRPTW: VRP with customer time windows.
- EVRP-TW: electric vehicle routing with time windows and charging constraints.
- Truck-drone collaborative VRP: synchronized mixed-fleet routing.

### 中文
- CVRP：容量约束车辆路径问题。
- VRPTW：带时间窗的车辆路径问题。
- EVRP-TW：考虑电量和充电约束的时间窗电动车路径问题。
- 卡车-无人机协同 VRP：多载具同步协同配送。

## 2. Core metrics | 核心指标

### EN
- Total cost or travel distance
- Feasibility rate
- Time-window violation count/penalty
- Energy consumption and charging count (EVRP)
- Makespan (especially for truck-drone collaboration)

### 中文
- 总成本或总路程
- 可行解比例
- 时间窗违约次数/惩罚
- 能耗与充电次数（EVRP）
- 完工时间（尤其适用于卡车-无人机协同）

## 3. Minimum reporting standard | 最低报告标准

### EN
Each team should report:
1. Baseline vs improved method on at least 3 instance sizes.
2. Feasibility and objective together (not objective only).
3. At least 3 failure cases and analysis.

### 中文
每个小组至少报告：
1. 在至少 3 种算例规模上比较基线与改进方法。
2. 同时报告可行性与目标值（不能只报目标值）。
3. 至少 3 个失败案例及其分析。
