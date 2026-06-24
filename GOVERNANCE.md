# UAGT Governance

UAGT aims to be a neutral, field-level reference — not a product or a marketing surface.
This document describes how the project is run and how decisions are made.

## Model

- The project currently operates under a **benevolent maintainer** model. The maintainer
  reviews and merges contributions and is responsible for the integrity of the crosswalk.
- The project lives in a **neutral home** (a dedicated GitHub org), independent of any
  single company. Sponsors and reference implementers may be acknowledged but do not
  control the framework.
- An **advisory group** may be convened to add review capacity and credibility.

## Review standard for mappings

Every change to a mapping must include:

1. A **rationale** explaining the correspondence.
2. A named **reviewer**.
3. A **relationship type** (`full` / `partial` / `superset` / `subset` / `none`) and a
   **confidence** level.

CI enforces the structural rules (schema validity, three-way coverage, version pins,
resolvable references). Human review covers the *judgment* in each mapping.

## Source manifest & versioning

The crosswalk is versioned with semantic versioning of the dataset:

- **MAJOR** — a source standard changes materially (e.g. the Digital Omnibus amendments
  land in the Official Journal and shift obligations).
- **MINOR** — controls or mappings are added.
- **PATCH** — corrections.

[`data/source-manifest.yaml`](data/source-manifest.yaml) pins the exact version/date of
each standard the current build reflects. Bumping a pin is a deliberate act and must be
accompanied by a changelog entry that narrates *why* a mapping moved — this living-document
behavior is the core value over static comparison tables.

## Evidence integrity

Adoption metrics are **organic only**. No purchased stars, no sockpuppets, no artificial
inflation. Every published number must be third-party-sourced, timestamped, and
reproducible. Manufactured adoption is both wrong and self-defeating for any evidentiary
use of this project.

## Decision-making

Day-to-day decisions rest with the maintainer. Significant changes (new frameworks,
schema changes, governance changes) should be proposed as an issue for discussion before
implementation. As the contributor base grows, this section will evolve toward a more
formal multi-maintainer model.
