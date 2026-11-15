# CR-SO-CAT-03: StrategicObjective Candidate Corpus

**Status**: Landed (this PR)
**Layer**: Catalog content (candidate corpus intake)
**Owner**: Emmanuel A. Otchere
**Date**: 2026-11-15
**Admission authority**: candidate corpus only (canonical admission remains the evidence-gated step; FOUNDATIONS D-4/D-5)
**Trigger**: Skeleton-advance wave (2026-11 owner directive): advance the remaining kit skeletons with evidence-backed candidate corpora through the gated intake workflow, grounded in the metamodel projection of this catalogue. the UN 2030 Agenda SDG framework (goals + targets, identifiers verbatim from the published framework) is the candidate seed source; corpus size honest-to-source (180).
**Carrier**: Single PR on feature branch `feat/cr-so-cat-03`. PR review, not direct push.
**Lands against**: `main`
**Depends on**: SO-CAT-02 (ingestion groundwork).

## 1. What this CR lands

**180 StrategicObjective candidate submissions** in `contributions/queue/<shard>/<slug>.yaml` from 1 evidence bank(s):

| Bank | Source | Records |
|---|---|---|
| un-sdg.json | UN 2030 Agenda SDG framework (goals + targets, sdgs.un.org) | 180 |

Provenance in `ingestion/manifest.yaml` (bank sha256s, source URLs, retrieval dates, mapping note). Every submission carries `source_ref`, a `published-document` evidence citation, and published description prose. Provisional field mappings are documented per record and in the manifest; per-organization values are canonical-admission decisions.


## 2. What changes

- `contributions/queue/<shard>/` — 180 intake submissions (`status: queued`)
- `ingestion/manifest.yaml` — corpus provenance record (new)
- No `CATALOG.yaml` change (queue ≠ index)
- This CR file and the index row

## 3. Verification

- `check_contributions.py`: CONFORMANT (180 queue files)
- No directory holds 800+ entries (slug-prefix distribution)
- Spot-checks: records trace to their published source identifiers

## 4. NOT-List

- NOT record admission (nothing under `entities/` changes; admission follows in SO-CAT-04+).
- NOT a modification of gates, schemas, or intake tooling.
- NOT an authoritative assessment of provisional mapped values.

## 5. Acceptance criteria

1. 180 gate-CONFORMANT submissions; manifest carries bank sha256s + source URLs.
2. Submissions carry no `id`; `status: queued`; `submitted_by: Emmanuel A. Otchere`.
3. `CATALOG.yaml` counts unchanged.
