# Project Outline (English)

## 1. Audience

Undergraduate students interested in optimization, operations research, AI, and logistics systems.

## 2. Prerequisites

- Python programming
- Basic optimization concepts (LP/IP helpful)
- Basic probability and statistics
- Familiarity with experiment reproducibility

## 3. Learning outcomes

By the end of this project, students can:

1. Explain VRP, CVRP, EVRP-TW, and truck-drone collaborative variants.
2. Reproduce at least one baseline solver or policy.
3. Evaluate methods with clear metrics and feasibility checks.
4. Analyze failure cases under realistic constraints.
5. Present technical findings with reproducible evidence.

## 4. Eight-week self-paced plan

### Week 1: Setup and orientation
- Environment setup and repository workflow
- Data format understanding
- Deliverable: setup checklist and successful smoke run

### Week 2: Fundamentals and literature mapping
- Read core VRP/EVRP references
- Build concept map for constraints/objectives
- Deliverable: reading memo

### Week 3: Baseline reproduction
- Reproduce one baseline (OR-Tools heuristic or RL baseline)
- Validate objective and feasibility outputs
- Deliverable: baseline logs

### Week 4: EVRP-TW focus
- Implement or run EVRP-TW experiments
- Track battery and time-window violations
- Deliverable: metrics table

### Week 5: Ground-air formulation
- Define truck-drone collaborative EVRP-TW model
- Clarify synchronization constraints
- Deliverable: formulation document

### Week 6: Hybrid solver implementation
- Implement heuristic/RL/hybrid method
- Test on small benchmark instances
- Deliverable: demo results

### Week 7: Improvement and ablation
- Improve one module (routing, charging, assignment)
- Run fair baseline comparison
- Deliverable: ablation and comparison table

### Week 8: Final integration
- Final report and reproducibility package
- Demo presentation
- Deliverable: final submission

## 5. Evaluation suggestion (non-class format)

- 25% Reproducibility and engineering quality
- 25% Baseline and improved-method comparison quality
- 20% Failure/error analysis depth
- 30% Final report and demo quality

## 6. Weekly operating rhythm

- Early week: define measurable objective
- Mid week: implement and run controlled experiments
- End week: summarize results and unresolved risks
- Optional mentor sync when blocked

## 7. Required final package

- Source code and scripts
- Config files and random seeds
- Logs/plots/tables for key experiments
- Final report (problem, method, results, limitations)
- Demo video (5-8 minutes)
