# 7.2-msql-grammar.md

Grammar (simplified):

QUERY := COMMAND ARGUMENTS

COMMAND ∈ {
  FIND,
  THREAD,
  RECALL,
  RECONSTRUCT
}

Examples:

FIND PATTERN "<pattern_label>"
THREAD "<thread_id>"
RECALL LAST <n> ENTRIES
