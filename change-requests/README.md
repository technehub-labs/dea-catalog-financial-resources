# Change Requests: dea-catalog-financial-resources

This index tracks every change request that lands on this repository.

| CR | Title | Status | Notes |
|----|-------|--------|-------|
| [CR-FR-CAT-01](CR-FR-CAT-01-catalogue-foundation.md) | Catalogue foundation (kit bring-up) | Landed (this PR) | Standard kit: pointer, dependencies, schema projection, gates 1-6, workflows, FOUNDATIONS, record standard. No records admitted. |
| CR-FR-CAT-02 | Initial population | Planned | Evidence-gated seed population per FOUNDATIONS §7. |

## Numbering

Series tag `CR-FR-CAT-NN`, sequential. Cross-repo CRs that touch this
repository are recorded here with their home-repo identifier.
| [CR-FR-CAT-02](CR-FR-CAT-02-cr-fr-cat-02.md) | Entity Ingestion Groundwork (candidate intake queue + gates) | **Proposed (this PR)** | Gated intake: queue + blocking queue gate + admission tool (candidate-state subtrees, content-derived ids); pin v2.6.0→v2.8.0 + shard-aware toolchain re-vendor. No records. |
| [CR-FR-CAT-03](CR-FR-CAT-03-cr-fr-cat-03.md) | FinancialResource Candidate Corpus | **Landed (this PR)** | 1500 queue submissions from 1 bank(s); manifest with sha256s; queue gate CONFORMANT; no entities change. |
| [CR-FR-CAT-01](CR-FR-CAT-01-cr-fr-cat-01.md) | FinancialResource Candidate Admission Batch 02 (AAAP — Pacer Barings CLO Market Flex ETF … COWG — Pacer US Large Cap Cash Cows Growth Leaders ETF) | **Landed (this PR)** | Admitted 1200 `FinancialResource` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +1200, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
| [CR-FR-CAT-02](CR-FR-CAT-02-cr-fr-cat-02.md) | FinancialResource Candidate Admission Batch 03 (COWS — Amplify Cash Flow Dividend Leaders ETF … DWAW — AdvisorShares Dorsey Wright FSM All Cap World ETF) | **Landed (this PR)** | Admitted 300 `FinancialResource` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +300, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
