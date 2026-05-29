# SOTA and Demo References | 前沿与示例项目

## 1. How to use references | 如何使用参考资料

### EN
- Start with one reproducible baseline.
- Improve one component at a time.
- Keep fairness: same instances, seeds, and evaluation pipeline.

### 中文
- 从一个可复现基线开始。
- 每次只改动一个模块。
- 公平对比：使用相同算例、随机种子和评测流程。

---

## 2. Representative papers | 代表性论文方向

### EN
- Deep reinforcement learning for VRP and EVRP variants.
- Learning-based heuristics and neural combinatorial optimization.
- Hybrid methods: RL + local search / metaheuristics.
- Truck-drone collaborative routing and synchronization constraints.

### 中文
- VRP/EVRP 的深度强化学习方法。
- 学习型启发式与神经组合优化。
- 混合方法：RL + 局部搜索/元启发式。
- 卡车-无人机协同路径与同步约束研究。

---

## 3. Demo repositories (starter set) | 示例仓库（起步清单）

- OR-Tools (Google): https://github.com/google/or-tools
- VRPy (Python VRP framework): https://github.com/Kuifje02/vrpy
- RL4CO (RL for combinatorial optimization): https://github.com/ai4co/rl4co
- PyVRP (metaheuristics for VRP): https://github.com/PyVRP/PyVRP
- HGS-CVRP implementation: https://github.com/vidalt/HGS-CVRP

For truck-drone keywords, start from GitHub search and filter by activity:
- https://github.com/search?q=truck+drone+routing&type=repositories

---

## 4. Suggested student path | 建议学生路径

### EN
1. Run OR-Tools baseline for CVRP/VRPTW.
2. Extend to EVRP-TW constraints.
3. Implement one RL or hybrid improvement.
4. Add truck-drone collaborative extension.
5. Compare quality/runtime/feasibility.

### 中文
1. 先跑通 OR-Tools 的 CVRP/VRPTW 基线。
2. 扩展到 EVRP-TW 约束。
3. 实现一个 RL 或混合改进。
4. 增加卡车-无人机协同扩展。
5. 比较解质量/耗时/可行性。
