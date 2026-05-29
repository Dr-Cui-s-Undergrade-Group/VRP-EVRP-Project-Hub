# SOTA, Demo, and Starter References

This page is a practical launchpad for SEP students working on VRP, EVRP-TW, neural combinatorial optimization, or truck-drone collaborative routing.

The recommended strategy: start with a classical baseline, then add constraints or learning components one at a time.

---

## 1. First Reading Path

1. **VRP and VRPTW basics**  
   Start with the OR-Tools routing tutorials to understand variables, constraints, dimensions, and feasibility reporting: [OR-Tools routing](https://developers.google.com/optimization/routing).

2. **Electric Vehicle Routing with Time Windows**  
   Read the classic EVRP-TW formulation: [The Electric Vehicle-Routing Problem with Time Windows and Recharging Stations](https://doi.org/10.1287/trsc.2013.0490).

3. **Neural combinatorial optimization**  
   Read [Attention, Learn to Solve Routing Problems](https://arxiv.org/abs/1803.08475) before POMO. It explains the attention model family used for TSP/VRP-style tasks.

4. **POMO**  
   Read [POMO: Policy Optimization with Multiple Optima for Reinforcement Learning](https://arxiv.org/abs/2010.16011) and inspect the [POMO code](https://github.com/yd-kwon/POMO).

5. **Truck-drone routing**  
   Start from the [Flying Sidekick Traveling Salesman Problem](https://doi.org/10.1287/trsc.2015.0605) to understand launch/recovery synchronization.

## 2. Starter Solvers and Codebases

| Resource | Use it for | Notes |
|---|---|---|
| [OR-Tools Routing](https://developers.google.com/optimization/routing) | First CVRP / VRPTW baseline | Reliable, well documented, good for Week 1. |
| [PyVRP](https://github.com/PyVRP/PyVRP) | High-quality VRP heuristic baseline | Strong practical baseline; includes examples and documentation. |
| [PyVRP docs](https://pyvrp.org/) | Tutorials and examples | Recommended for students who want a Python-first solver. |
| [POMO](https://github.com/yd-kwon/POMO) | RL baseline for TSP/CVRP-style tasks | Required reference for learning-based route construction. |
| [Attention Learn to Route](https://github.com/wouterkool/attention-learn-to-route) | Attention model baseline | Good background for neural construction policies. |
| [RL4CO](https://github.com/ai4co/rl4co) | Modern RL-for-combinatorial-optimization framework | Useful for experiments beyond one paper's codebase. |
| [HGS-CVRP](https://github.com/vidalt/HGS-CVRP) | Strong classical CVRP baseline | Useful for understanding how strong heuristics behave. |

## 3. Problem Variants

| Variant | What changes | Good first metric |
|---|---|---|
| CVRP | vehicle capacity only | total distance and feasibility |
| VRPTW | customer time windows | total distance plus time-window violations |
| EVRP-TW | battery, charging, time windows | feasibility, charging count, energy violations |
| Truck-drone VRP | synchronized ground-air delivery | makespan, synchronization violations |

Do not jump directly to truck-drone EVRP-TW unless a simpler VRPTW baseline already runs.

## 4. Benchmarks and Data

Useful places to look:

- [OR-Tools routing examples](https://developers.google.com/optimization/routing)
- [PyVRP examples](https://pyvrp.org/examples/index.html)
- [VRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/)
- Solomon-style VRPTW instances, often used in routing literature.
- Schneider EVRP-TW benchmark instances, associated with the EVRP-TW paper.

When using any benchmark, document the exact source, instance name, scaling convention, and any preprocessing.

## 5. Videos and Demo Pages

GitHub README files do not reliably support embedded video playback. For direct browser playback and demo links, see [`media.html`](media.html). Useful external pages:

- [Google OR-Tools routing guides](https://developers.google.com/optimization/routing)
- [PyVRP examples](https://pyvrp.org/examples/index.html)
- [BCS video page: Introduction to Operations Research with Google OR-Tools](https://www.bcs.org/events-calendar/2026/march/hybrid-an-introduction-to-operations-research-with-google-or-tools/)
- [RL4CO documentation](https://rl4co.readthedocs.io/)

## 6. Suggested Baseline Choices

Choose one:

1. **OR-Tools VRPTW baseline**  
   Best for learning constraints and producing a clear feasibility report.

2. **PyVRP CVRP / VRPTW baseline**  
   Best for a strong practical solver and clean Python experiments.

3. **POMO CVRP baseline**  
   Best for students who specifically want reinforcement learning and neural combinatorial optimization.

4. **Small truck-drone heuristic**  
   Best for students with good optimization background. Start with tiny handcrafted instances and clear synchronization rules.

## 7. Minimum Implementation Goal

A project is acceptable only when it includes:

- a runnable baseline command;
- instance files or instance-generation code;
- objective value, feasibility status, and runtime;
- at least 3 instance sizes or 3 representative instances;
- one improvement or extension;
- failure cases explaining constraint violations.

## 8. Search Keywords

Useful keywords for further reading:

- `Electric Vehicle Routing Problem with Time Windows`
- `EVRP-TW recharging stations`
- `POMO CVRP reinforcement learning`
- `neural combinatorial optimization vehicle routing`
- `PyVRP vehicle routing`
- `truck drone routing synchronization`
- `Flying Sidekick Traveling Salesman Problem`

Strong routing work is usually careful, not flashy. Always compare against a simple baseline first.
