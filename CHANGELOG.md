# Changelog

All notable changes to this catalog are documented here. Format follows
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### CR-FR-CAT-02: FinancialResource Candidate Admission Batch 03

Admitted 300 new `FinancialResource` CANDIDATE records through the gated intake workflow (queue gate → admission tool → catalog gates); ids content-derived and collision-checked; records land in `candidates/` subtrees at `lifecycle_status: proposed` / version 0.1.0; candidates count +300, canonical unchanged; queue entries flipped to `admitted`.

### CR-FR-CAT-01: FinancialResource Candidate Admission Batch 02

Admitted 1200 new `FinancialResource` CANDIDATE records through the gated intake workflow (queue gate → admission tool → catalog gates); ids content-derived and collision-checked; records land in `candidates/` subtrees at `lifecycle_status: proposed` / version 0.1.0; candidates count +1200, canonical unchanged; queue entries flipped to `admitted`.

### CR-FR-CAT-03: FinancialResource Candidate Corpus

1500 FinancialResource candidate submissions landed in the contribution queue (sharded, gate-CONFORMANT) from 1 evidence bank(s); published prose + evidence citations + source_refs; provenance in ingestion/manifest.yaml. No catalog entities change; admission follows in FR-CAT-04+.

### CR-FR-CAT-02: Entity Ingestion Groundwork (candidate intake queue + gates)

Gated intake workflow stood up: contribution queue + blocking queue gate (`scripts/check_contributions.py`, self-deriving from the projected schema) + admission tool (`scripts/admit_entity.py`: content-derived ids, collision-checked, candidates/ subtrees at `lifecycle_status: proposed` / v0.1.0) + intake template and process docs. CI: queue gate added as a blocking step; metaframework pin v2.6.0 → v2.8.0 with the shard-aware toolchain re-vendored from the v2.8.0 release (cmp'd). No records admitted by this CR.

### Added

- Catalog bootstrapped from `dea-metaframework/tools/catalog-repo-template/`
  (TEMPLATE_VERSION 0.1.0). Authored under CR-CATALOG-STRUCT-06b.
