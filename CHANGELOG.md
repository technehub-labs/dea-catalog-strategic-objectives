# Changelog

## [Unreleased]

### CR-SO-CAT-05: Canonical Admission Wave

180 StrategicObjective records promoted from the candidate slot to the canonical slot (provenance ladder completed per record; evidence citations preserved; ids untouched). Index: canonical 180, candidates 0. All gates green.

### CR-SO-CAT-04: StrategicObjective Candidate Admission Batch 05

Admitted 180 new `StrategicObjective` CANDIDATE records through the gated intake workflow (queue gate → admission tool → catalog gates); ids content-derived and collision-checked; records land in `candidates/` subtrees at `lifecycle_status: proposed` / version 0.1.0; candidates count +180, canonical unchanged; queue entries flipped to `admitted`.

### CR-SO-CAT-03: StrategicObjective Candidate Corpus

180 StrategicObjective candidate submissions landed in the contribution queue (sharded, gate-CONFORMANT) from 1 evidence bank(s); published prose + evidence citations + source_refs; provenance in ingestion/manifest.yaml. No catalog entities change; admission follows in SO-CAT-04+.

### CR-SO-CAT-02: Entity Ingestion Groundwork (candidate intake queue + gates)

Gated intake workflow stood up: contribution queue + blocking queue gate (`scripts/check_contributions.py`, self-deriving from the projected schema) + admission tool (`scripts/admit_entity.py`: content-derived ids, collision-checked, candidates/ subtrees at `lifecycle_status: proposed` / v0.1.0) + intake template and process docs. CI: queue gate added as a blocking step; metaframework pin v2.6.0 → v2.8.0 with the shard-aware toolchain re-vendored from the v2.8.0 release (cmp'd). No records admitted by this CR.

### `CR-SO-CAT-01` — catalogue foundation (kit bring-up)

Standard kit generated from the metamodel (org-wide catalog advancement
programme): hybrid pointer pinned to OpenDEAM v0.8.0;
`dependencies.yaml`; schema projection (derived-from-entity-definition) with the
catalogue-instance layer; vendored relationship-instance contract; fixtures;
gates 1-6 wired into `validate-catalogue.yml` plus allocation and authorship
workflows; FOUNDATIONS (D-1..D-6) and record documentation standard. No
records admitted (population gated on CR-SO-CAT-02).
