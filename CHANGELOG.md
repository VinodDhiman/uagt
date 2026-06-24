# Changelog

All notable changes to the UAGC crosswalk are recorded here. The changelog narrates
*why* a mapping moved — especially as source standards shift — which is the living-document
value static comparison tables cannot match.

The format is based on [Keep a Changelog](https://keepachangelog.com/), and the dataset
uses semantic versioning (see [GOVERNANCE.md](GOVERNANCE.md)): MAJOR for material source-
standard changes, MINOR for added controls/mappings, PATCH for corrections.

## [Unreleased]

### Added
- Initial repository scaffolding: JSON Schema, source manifest, build pipeline
  (`scripts/build_tables.py`), governance/contribution/license files, and CI.
- Sample Master Controls across four domains: `MC-RM-01`, `MC-DG-03`, `MC-HO-01`,
  and `MC-TR-02` (the latter demonstrating a `none` gap — an EU AI Act Art.50 obligation
  with no clean ISO/NIST equivalent).

### Tracking
- **EU AI Act — Digital Omnibus on AI:** provisional political agreement reached
  7 May 2026; formal adoption expected ~June–July 2026. The source manifest currently
  reflects Regulation (EU) 2024/1689 as enacted. Official Journal publication of the
  Omnibus will trigger a MAJOR version bump and re-review of affected mappings.
