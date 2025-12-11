---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/String
generated: 2025-12-11T21:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# String

## Overview

The `String/` directory provides additional definitions, lemmas, and order-theoretic structure for Lean's built-in `String` type in mathlib4. It extends strings with padding operations (`leftpad`, `rightpad`, `replicate`), prefix/suffix predicates (`IsPrefix`, `IsSuffix`), token mapping utilities, and establishes a `LinearOrder` instance on strings based on lexicographic ordering of their underlying character lists. The implementation connects string operations to their `List Char` counterparts, enabling proof techniques that leverage list reasoning.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core string definitions: `leftpad`, `rightpad`, `replicate` for padding; `IsPrefix`, `IsSuffix` predicates; `mapTokens` for tokenization; `head` accessor |
| Lemmas.lean | Lemmas about string operations: `length_replicate`, `length_leftpad`, `leftpad_prefix`, `leftpad_suffix`, and `congr_append` |
| Basic.lean | `LinearOrder` instance for strings via lexicographic comparison; defines `ltb` for comparing string iterators; proves `lt_iff_toList_lt` and `le_iff_toList_le` connecting string ordering to list ordering |

## Subdirectories

*(none)*

## Search Tags

string strings padding leftpad rightpad replicate prefix suffix linearorder lexicographic comparison isprefix issuffix maptokens tokenization
