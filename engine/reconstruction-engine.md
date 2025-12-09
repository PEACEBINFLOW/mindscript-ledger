# 6.4-reconstruction-engine.md

Reconstruction takes:

- a thread_id or entry range
- reads entries in order
- optionally applies snapshots + deltas

It returns:

- ordered list of inputs
- derived session summary
- list of pattern hashes involved
