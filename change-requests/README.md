# Change Requests: dea-catalog-strategic-objectives

This index tracks every change request that lands on this repository.

| CR | Title | Status | Notes |
|----|-------|--------|-------|
| [CR-SO-CAT-01](CR-SO-CAT-01-catalogue-foundation.md) | Catalogue foundation (kit bring-up) | Landed (this PR) | Standard kit: pointer, dependencies, schema projection, gates 1-6, workflows, FOUNDATIONS, record standard. No records admitted. |
| CR-SO-CAT-02 | Initial population | Planned | Evidence-gated seed population per FOUNDATIONS §7. |

## Numbering

Series tag `CR-SO-CAT-NN`, sequential. Cross-repo CRs that touch this
repository are recorded here with their home-repo identifier.
| [CR-SO-CAT-02](CR-SO-CAT-02-cr-so-cat-02.md) | Entity Ingestion Groundwork (candidate intake queue + gates) | **Proposed (this PR)** | Gated intake: queue + blocking queue gate + admission tool (candidate-state subtrees, content-derived ids); pin v2.6.0→v2.8.0 + shard-aware toolchain re-vendor. No records. |
| [CR-SO-CAT-03](CR-SO-CAT-03-cr-so-cat-03.md) | StrategicObjective Candidate Corpus | **Landed (this PR)** | 180 queue submissions from 1 bank(s); manifest with sha256s; queue gate CONFORMANT; no entities change. |
| [CR-SO-CAT-04](CR-SO-CAT-04-cr-so-cat-04.md) | StrategicObjective Candidate Admission Batch 05 (SDG 1: No Poverty … SDG Target 9.8 (Industry, Innovation and Infrastructure)) | **Landed (this PR)** | Admitted 180 `StrategicObjective` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +180, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
