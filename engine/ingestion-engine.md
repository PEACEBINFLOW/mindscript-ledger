# 6.1-ingestion-engine.md

Ingestion steps:

1. Receive raw input + context
2. Normalize input
3. Compute pattern_hash
4. Assign thread_id (existing or new)
5. Create LedgerEntry object
6. Persist entry + update thread + update pattern node
