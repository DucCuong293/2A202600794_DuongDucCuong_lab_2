# Day 02 AI Product Lab - 2A202600794 Duong Duc Cuong

This repository contains my Day 02 AI Product Lab submission. The lab focuses on finding the right problem for AI before jumping into a solution.

## Project Topic

Selected everyday problem:

```text
Students living away from home spend too much time deciding what to eat, often buy too much or too little food, and struggle to keep food spending stable.
```

The chosen direction is a lightweight AI-supported workflow, not a fully autonomous agent. AI helps suggest meals and a shopping list, while the student still reviews budget, taste, ingredients, and the final decision.

## Repository Structure

```text
Day02_2A202600794_DuongDucCuong/
├── README.md
├── 01-individual-problem-scan/
│   ├── 01-individual-problem.md
│   └── 01-individual-problem-scan-workflow-card-1.png
├── 02-group-problem-statement/
│   ├── 02-group-problem-statement.md
│   ├── 02-group-problem-statement-research-notes.md
│   └── 02-group-problem-statement-workflow.pdf
└── 03-individual-reflection/
    └── 03-individual-reflection.md
```

## Deliverables

| Part | File | Description |
|---|---|---|
| 01 - Individual Problem Scan | `01-individual-problem.md` | Scans 10 everyday problems, selects the top 3, and develops detailed Problem Cards. |
| Workflow Card | `01-individual-problem-scan-workflow-card-1.png` | Visual before/after workflow for Problem Card #1. |
| 02 - Group Problem Statement | `02-group-problem-statement.md` | Shows group convergence, shortlist scoring, validation, workflow, Problem Statement v0/v1, Rule/Workflow/Agent comparison, and final decision. |
| Research Notes | `02-group-problem-statement-research-notes.md` | Records research sources, patterns, risks, metrics, and why Workflow is preferred over Agent. |
| Workflow PDF | `02-group-problem-statement-workflow.pdf` | Visual workflow artifact for the group problem statement. |
| 03 - Individual Reflection | `03-individual-reflection.md` | Reflects on personal contribution, AI usage, lessons learned, and what I would improve next time. |

## Final Decision

```text
Go with a small-scope Workflow.
```

Why:

- The actor is clear: students living away from home and preparing meals 3-5 times per week.
- The current workflow is observable and repeated.
- The bottleneck is specific: deciding what to eat and making a shopping list.
- Success can be measured by time saved and fewer missing/extra ingredients.
- AI supports one concrete step instead of taking over the whole food workflow.
- Human review remains the boundary before buying food.

## Rule / Workflow / Agent Summary

| Level | Role in this project |
|---|---|
| No AI / Process fix | Fixed menu and shopping checklist as a fallback. |
| Rule | Filter familiar meals by budget, cooking time, and ingredient constraints. |
| Workflow | Chosen approach: user input -> AI meal suggestions -> AI shopping list -> human review. |
| Agent | Not chosen because autonomous meal planning or ordering is too broad and risky for this lab scope. |

## Key Success Metrics

| Metric | Baseline | Target |
|---|---:|---:|
| Time to decide meal and shopping list | About 35 minutes | Under 10 minutes |
| Missing/extra ingredient incidents | 2-3 times per week | 0-1 time per week |
| Pilot duration | Not yet measured | 1 week |

## Notes

This is a lab submission, not a production application. The goal is to demonstrate problem framing, workflow analysis, AI fit reasoning, and a clear decision between Rule, Workflow, and Agent.
