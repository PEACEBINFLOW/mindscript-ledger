# mindscript-ledger  
### Temporal Ledger & Recall Engine for MindScript  
by **Peace Thabiwa — SAGEWORKS AI**

---

## What is MindScript Ledger?

MindScript Ledger is the memory fabric for the MindScript ecosystem.

Instead of relying on raw chat history, it stores:

- normalized prompts (inputs)
- logic and stage metadata
- pattern hashes
- temporal order
- threads of interaction
- snapshots and deltas

This lets you:

- reconstruct past sessions deterministically  
- recall patterns instead of keywords  
- replay state transitions  
- share memory across different AI models (GPT, Gemini, etc.)

---

## Repo Contents

- `2-OVERVIEW.md` — conceptual overview  
- `3-spec/` — full ledger model specification  
- `4-schemas/` — JSON schemas for entries, threads, patterns, snapshots  
- `5-storage/` — storage layout + compaction rules  
- `6-engine/` — ingestion, state machine, reconstruction docs  
- `7-query-language/` — MSQL (MindScript Query Language)  
- `8-integrations/` — how this binds to MindScript Core + Templates  
- `9-examples/` — concrete example files  
- `10-roadmap.md` — future plans

---

## Status

- v0.1 — Specification + schemas  
- v0.2 — Reference implementations (planned)  
- v1.0 — Production-ready engine (future)

---

## Ecosystem

MindScript repos:

- `mindscript-core` — language spec & laws  
- `mindscript-templates` — multimodal templates  
- `mindscript-ledger` — this repo, temporal memory layer  
