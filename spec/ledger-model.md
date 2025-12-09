# 3.1-ledger-model.md  
## Ledger Data Model

The ledger data model is built around four primary objects:

1. **Entry**
2. **Thread**
3. **PatternNode**
4. **Snapshot**

### 1. Entry

Represents a single atomic interaction.

Fields:
- `id` — unique identifier
- `timestamp` — ISO8601
- `input` — normalized user or system input
- `output_ref` — optional reference to output
- `pattern_hash` — hash representing logical shape
- `stage` — numeric or symbolic stage
- `logic_block` — short label for the logic segment
- `thread_id` — which thread this belongs to
- `links` — prev/next relationships

---

### 2. Thread

Represents a chain of entries.

- `thread_id`
- `root_entry_id`
- `entry_ids[]`
- `tags[]`
- `summary`

---

### 3. PatternNode

Represents a reusable pattern (e.g., "5-stage essay generation").

- `pattern_hash`
- `description`
- `frequency`
- `first_seen_at`
- `last_seen_at`
- `examples[]`

---

### 4. Snapshot

Represents a compressed view of state at a given time.

- `snapshot_id`
- `timestamp`
- `thread_id`
- `entry_range`
- `state_summary`
