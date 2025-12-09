# 5.1-storage-layout.md

Recommended on-disk structure:

/ledger/
  /entries/
    YYYY/
      MM/
        DD/
          <entry_id>.json
  /threads/
    <thread_id>.json
  /patterns/
    <pattern_hash>.json
  /snapshots/
    <snapshot_id>.json
