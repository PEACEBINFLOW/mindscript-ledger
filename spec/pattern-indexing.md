## Pattern Indexing

Pattern hash is defined as:

```text
pattern_hash = HASH(
  normalize(input) +
  "|" +
  logic_block +
  "|" +
  stage
)
normalize(input) — lowercased, trimmed, structural tokens preserved.

logic_block — short label (e.g., name_list_generator).

stage — stage number or name.

Goals:

identical logical prompts → identical pattern hash

minor wording drift → still close in pattern tree
