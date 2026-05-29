# Project Outline: VRP, EVRP-TW, and Truck-Drone Routing

## 1. Audience

This SEP research project is designed for undergraduate students interested in optimization, operations research, logistics systems, artificial intelligence, or reinforcement learning for combinatorial problems.

The project is suitable for students who want to understand how routing algorithms make decisions under real constraints such as capacity, time windows, battery limits, charging stations, and synchronized truck-drone delivery.

## 2. Prerequisites

Students are expected to have:

- Python programming skills;
- basic probability and statistics;
- willingness to read papers and run experiments carefully;
- basic understanding of algorithms.

Helpful but not required:

- linear programming or integer programming;
- graph algorithms;
- PyTorch;
- reinforcement learning;
- operations research background.

## 3. Learning Outcomes

By the end of the project, students should be able to:

1. Explain CVRP, VRPTW, EVRP-TW, and truck-drone routing variants.
2. Reproduce one baseline solver or learning-based policy.
3. Report objective value, feasibility, constraint violations, and runtime.
4. Diagnose why a route is infeasible or inefficient.
5. Implement one focused improvement or extension.
6. Present a reproducible optimization experiment with clear evidence.

## 4. Research Tracks

| Track | Main question | Typical tools |
|---|---|---|
| Classical VRP / VRPTW | How do standard solvers handle capacity and time windows? | OR-Tools, PyVRP |
| Deep RL for EVRP-TW | Can a learned policy construct feasible electric-vehicle routes? | POMO, Attention Model, RL4CO |
| Hybrid EVRP-TW | Can learning and local search repair or improve each other? | PyVRP, custom repair heuristics, neural construction |
| Truck-drone Routing | How should ground and aerial vehicles synchronize service? | small custom instances, heuristic search, makespan analysis |

Students should start from a simple baseline before adding battery or drone constraints.

## 5. Eight-Week Plan

| Week | Focus | Deliverable |
|---|---|---|
| 1 | Environment and baseline setup | one solved tiny instance |
| 2 | Problem variants and literature | reading notes and constraint diagram |
| 3 | Baseline reproduction | objective, feasibility, runtime logs |
| 4 | EVRP-TW constraints | time-window and battery violation table |
| 5 | Truck-drone formulation | model note and synchronization rules |
| 6 | Hybrid or learning method | demo run on small instances |
| 7 | Improvement and ablation | fair comparison with baseline |
| 8 | Final integration | report, slides, demo video, reproducibility package |

## 6. Assessment Guidance

Suggested assessment weights:

- 25% reproducibility and engineering quality;
- 25% baseline and improved method comparison;
- 20% failure or constraint-violation analysis;
- 30% final report, demo, and technical explanation.

## 7. Final Submission

The final package should include:

- source code or runnable scripts;
- instance files or generation scripts;
- solver/model configs and random seeds;
- objective, feasibility, runtime, and violation tables;
- route plots or textual route outputs;
- failure analysis;
- final report and 5-8 minute presentation video.

## 8. Recommended First Step

Read [SOTA and demo references](sota_demo_references.md), choose OR-Tools or PyVRP for the first baseline, and complete [Week 1 Lab](../labs/week01_setup.md). A feasible route with clear logs is the first milestone.
