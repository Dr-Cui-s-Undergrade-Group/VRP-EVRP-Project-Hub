# Four-Project Relationship Map | 四个课题关系图

This page explains why four project topics are organized into two repositories.  
本页说明为什么四个课题会被组织为两个仓库。

## 1. Portfolio view | 全局视角

### EN

The four topics naturally form two technical families:

- Family A (Embodied Navigation): language/vision/perception/control on mobile robots.
- Family B (Routing Optimization): combinatorial optimization for logistics under constraints.

So we use two repositories to keep learning paths clear while preserving collaboration links.

### 中文

这四个课题自然分成两个技术家族：

- A 类（具身导航）：移动机器人中的语言/视觉/感知/控制。
- B 类（路径优化）：约束物流场景下的组合优化。

因此用两个仓库来保持学习路径清晰，同时保留跨项目协作关系。

---

## 2. Exact mapping | 精确映射

| Project in project.txt | Primary Repo | Why |
|---|---|---|
| Vision-Language Navigation for an AMR | VLN-AMR-Bootcamp-2026 | Core VLN task: language-to-action navigation |
| End-to-End Navigation for an AMR with RL | VLN-AMR-Bootcamp-2026 | Same robot navigation stack, different learning paradigm |
| Deep RL for EVRP-TW | VRP-EVRP-Bootcamp-2026 | Routing optimization with EV and time-window constraints |
| Ground-Air Collaborative EVRP-TW | VRP-EVRP-Bootcamp-2026 | Extension of EVRP-TW to truck-drone collaboration |

---

## 3. How the four projects connect | 四个课题如何关联

### EN

- Projects 1 and 4 share robotics deployment concerns: state estimation, policy stability, sim-to-real thinking.
- Projects 2 and 3 share optimization concerns: feasibility, objective trade-offs, scalable solvers.
- Cross-family connection: navigation outputs can inform delivery execution, while routing plans can provide high-level goals to robot navigation systems.

### 中文

- 课题 1 和 4 共享机器人落地问题：状态估计、策略稳定性、仿真到现实。
- 课题 2 和 3 共享优化问题：可行性、目标权衡、可扩展求解。
- 跨家族联系：导航系统可执行配送动作，路径优化可提供高层任务目标。

---

## 4. Student guidance | 学生选题建议

### EN

- If you like robotics perception/control: start in VLN-AMR-Bootcamp-2026.
- If you like optimization/logistics: start in VRP-EVRP-Bootcamp-2026.
- For capstone-level depth: pick one primary track and one cross-track integration question.

### 中文

- 偏好机器人感知/控制：从 VLN-AMR-Bootcamp-2026 开始。
- 偏好优化/物流：从 VRP-EVRP-Bootcamp-2026 开始。
- 若做高阶整合：主修一个方向，再增加一个跨方向融合问题。
