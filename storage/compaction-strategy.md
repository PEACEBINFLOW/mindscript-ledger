# 5.3-compaction-strategy.md

Compaction goals:

- reduce file count
- merge old entries into snapshots
- keep recent data granular

Strategies:
- periodic snapshot creation
- merging small entries into segment files
- pruning dead threads if allowed
