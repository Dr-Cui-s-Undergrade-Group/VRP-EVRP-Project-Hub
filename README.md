# 🚚⚡ VRP/EVRP Project Hub (Self-Paced)

From classical routing to learning-based and truck-drone collaborative optimization.

Start Here · [English Project Outline](docs/project_outline_en.md) · [中文项目大纲](docs/project_outline_zh.md) · [How to Ask Questions / 如何提问](docs/asking_questions.md) · [Benchmarks and Metrics / 基准与指标](docs/benchmarks_metrics_bilingual.md) · [SOTA and Demo References / 前沿与示例项目](docs/sota_demo_references.md) · [4 Projects Relationship Map / 四项目关系图](docs/four_project_relationship_map.md)

---

## 🌟 Why this project exists | 为什么做这个项目

**EN**
Vehicle Routing Problems (VRP) are at the core of modern logistics.
In realistic scenarios, constraints such as time windows, battery limits, and mixed fleets (truck + drone) make optimization much harder and much more relevant.

This repository helps undergraduate students build practical routing research skills through reproducible experiments.

**中文**
车辆路径问题（VRP）是现代物流优化的核心问题。
在真实场景中，时间窗、电池约束、混合车队（卡车+无人机）等条件会显著增加难度，也更贴近应用。

本仓库面向本科生，通过可复现实验训练路径优化与科研实践能力。

---

## 🎯 Project tracks | 项目方向

**Track A: Deep RL for EVRP-TW**
- Learn a policy to solve Electric Vehicle Routing with Time Windows.
- Focus on battery-aware decisions, recharge strategy, and feasibility.

**Track B: Ground-Air Collaborative EVRP-TW**
- Hybrid optimization for truck-drone delivery.
- Focus on coordination, launch/recovery constraints, and makespan/cost trade-off.

---

## 🔗 Why 4 projects are in 2 repositories | 为什么 4 个课题对应 2 个仓库

| Topic from project.txt | This repo role | Sister repo role |
|---|---|---|
| Deep RL for EVRP-TW | Primary home (EVRP-TW) | Provides robot execution perspective |
| Ground-Air Collaborative EVRP-TW | Primary home (truck-drone collaboration) | Provides autonomy and navigation insights |
| Vision-Language Navigation for an AMR | Uses routing goals as high-level tasks | Primary home |
| End-to-End Navigation for an AMR with RL | Uses route plans as decision context | Primary home |

See full explanation: [4 Projects Relationship Map / 四项目关系图](docs/four_project_relationship_map.md)

---

## 🧭 Start here | 从这里开始

| Role / 场景 | What to read / 建议阅读 |
|---|---|
| New student / 新同学 | [English Project Outline](docs/project_outline_en.md) and [中文项目大纲](docs/project_outline_zh.md) |
| Need question format / 不知道怎么提问 | [How to Ask Questions / 如何提问](docs/asking_questions.md) |
| Need references / 想看参考资料 | [SOTA and Demo References / 前沿与示例项目](docs/sota_demo_references.md) |
| Need evaluation rules / 想看评估方法 | [Benchmarks and Metrics / 基准与指标](docs/benchmarks_metrics_bilingual.md) |

---

## 🗓️ Suggested 8-week self-paced roadmap | 建议 8 周自驱路线

| Week | Theme (EN) | 主题（中文） | Deliverable |
|---|---|---|---|
| 1 | Environment and baseline setup | 环境搭建与基线准备 | Setup evidence |
| 2 | VRP/EVRP fundamentals and paper reading | VRP/EVRP 基础与论文阅读 | Reading note |
| 3 | Reproduce one baseline solver | 复现一个基线求解器 | Reproduction logs |
| 4 | EVRP-TW training/evaluation | EVRP-TW 训练与评估 | Metrics table |
| 5 | Truck-drone hybrid formulation | 卡车-无人机协同建模 | Problem formulation note |
| 6 | Hybrid algorithm implementation | 协同算法实现与调试 | Demo run |
| 7 | Improvement and ablation | 改进与消融实验 | Comparison table |
| 8 | Final report and demo | 最终报告与演示 | Final package |

---

## 🔁 Weekly workflow (no formal classes) | 每周推进方式（无正式授课）

**EN**
- Day 1-2: lock weekly objective and baseline
- Day 3-4: run experiments and track failures
- Day 5: summarize results and open issues
- Weekend: optional mentor sync / peer review

**中文**
- 第 1-2 天：明确本周目标和基线
- 第 3-4 天：实验运行并记录失败案例
- 第 5 天：总结结果并更新问题清单
- 周末：可选导师沟通或同伴互评

---

## 📦 Repository structure | 仓库结构

```text
VRP-EVRP-Bootcamp-2026/
├── README.md
├── docs/
│   ├── project_outline_en.md
│   ├── project_outline_zh.md
│   ├── asking_questions.md
│   ├── benchmarks_metrics_bilingual.md
│   ├── sota_demo_references.md
│   └── four_project_relationship_map.md
├── labs/
├── assignments/
├── checklists/
├── resources/
├── slides/
├── assets/
└── .github/
    └── ISSUE_TEMPLATE/
```

---

## 🏁 Final destination | 最终目标

**EN**
A strong team can not only report one good number, but also explain:
- why the method works,
- where it fails,
- and which evidence supports next-step improvements.

**中文**
优秀团队不只是给出一个“最好结果”，而是能够解释：
- 方法为什么有效，
- 在哪里失效，
- 下一步改进由哪些证据支持。
