# 6.3-state-machine.md

State transitions for a thread:

NEW → ACTIVE → SNAPSHOTTED → ARCHIVED

Each new entry updates:
- current stage
- last_activity timestamp
