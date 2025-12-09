# 2-OVERVIEW.md  
## High-Level Concept

The MindScript Ledger acts as a **time-stamped pattern log**.

Key properties:

- **Pattern-based**: every entry is indexed by a pattern hash derived from the normalized input and logic.
- **Temporal**: entries are ordered in time and linked into threads.
- **Deterministic**: given the same set of entries + templates, you can reconstruct a previous reasoning sequence.

Core entities:

- **Ledger Entry** — one atomic step (input + meta).
- **Thread** — ordered list of entries with links.
- **Pattern Node** — record of a reusable pattern.
- **Snapshot** — compressed view of a state at time T.

The Ledger is designed for AI-native workflows like:

- “Rebuild the session where I designed MindScript v1.”  
- “Recall all pattern usages for my ‘multi-stage essay’ template.”  
- “Replay only stages that matched a specific logic block.”
