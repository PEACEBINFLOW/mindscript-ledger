# 3.2-entry-types.md  
## Entry Types

Entries can be categorized by type:

- `input_only` — pure input, no output captured
- `input_output` — input with stable output reference
- `system_event` —-engine or environment events
- `snapshot_marker` — denotes where a snapshot was captured

Field: `entry_type` (string)

Examples:
- `"input_only"`
- `"input_output"`
- `"system_event"`
- `"snapshot_marker"`
