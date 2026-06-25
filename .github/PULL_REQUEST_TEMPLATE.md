<!-- Thanks for contributing to UAGT. Keep PRs focused (ideally one control or one
     coherent set of mappings). See CONTRIBUTING.md and GOVERNANCE.md. -->

## What this changes

<!-- One or two sentences. Which control(s) / mapping(s) / framework(s)? -->

## Mapping rationale (required for any mapping change)

<!-- For each changed mapping: the relationship (full/partial/superset/subset/none),
     a short defensible rationale, and your reviewer name. -->

## Checklist

- [ ] I did **not** paste source-standard text (identifiers + short labels only)
- [ ] Every changed mapping has a **relationship**, **rationale**, **confidence**, and **reviewer**
- [ ] All three frameworks are present for each control (or explicitly `relationship: none`)
- [ ] `version` matches the pinned value in `data/source-manifest.yaml`
- [ ] `python scripts/build_tables.py --check` passes locally
- [ ] `python -m pytest -q` passes locally
- [ ] I regenerated and committed `docs/` (`python scripts/build_tables.py`)
