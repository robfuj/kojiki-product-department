# 07 — Product

> Part of the **Hermes Organizational Decision System**. This repo is the
> **Product** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/hermes-ios/00-kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> What should we create?

## Purpose
Identify valuable problems, prioritize investments, and validate solutions.

## Sub-functions
Product Strategy, Product Management, Product Operations, User Research, Product Design, UX, Product Analytics, Product Growth

## Typical roles
CPO, VP Product, Head of Product, Product Director, Group Product Manager, Product Manager, Product Owner, Product Operations Manager, UX Researcher

## Inputs
Customer problems, research, usage data, market signals, technical constraints, economics.

## Outputs
Roadmaps, product decisions, requirements, experiments, product outcomes.

## Learning focus
Problem patterns; user behavior; product-market-fit signals; experiment quality; adoption; prioritization accuracy.

## Operating tree
```text
OBSERVATION →
    PROBLEM →
    USER →
    HYPOTHESIS →
    RESEARCH →
    VALIDATION →
    PRIORITIZATION →
    SOLUTION →
    EXPERIMENT →
    MEASUREMENT →
    DECISION →
    LEARNING
```

## Decision states
```text
OBSERVED → RESEARCHING → VALIDATED → PRIORITIZED → BUILDING → EXPERIMENTING → SHIPPED → ITERATING → KILLED
```

## Decision outputs
`Investigate · Validate · Build · Iterate · Prioritize · Kill`

## Critical prompts (what this function thinks about)
> What problem are we observing?
> Who has this problem?
> How frequently?
> How painful is it?
> What happens if nothing changes?
> How are users solving it today?
> Why is the current solution inadequate?
> What evidence proves the problem exists?
> What assumptions are we making?
> Which assumption is most dangerous?
> What is the cheapest experiment?
> What would falsify the hypothesis?
> What should we build?
> What should we not build?
> What metric should change?
> Did behavior actually change?
> Did we solve the problem?
> What did users teach us?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/07-product.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
