---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/FinEnum
generated: 2025-12-09T04:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 1
subdirs_count: 0
---

# FinEnum

## Overview

The `FinEnum/` subdirectory extends the `FinEnum` type class (finitely enumerable types with explicit bijections to `Fin n`) with additional instances and recursion principles. Currently contains support for `Option` types, providing a recursor analogous to `Nat.rec` that can construct data (not just proofs) by treating every `FinEnum` as either `Empty` or `Option α`. This enables more powerful inductive constructions than the `Fintype` version since data can be transported along equivalences mediated by `Fin`.

## Key Files

| File | Purpose |
|------|---------|
| Option.lean | `FinEnum` instance for `Option α` types; provides `recEmptyOption` recursor that says every `FinEnum` is either `PEmpty` or `Option α` up to equivalence, allowing data transport (unlike `Fintype` which only works for `Prop`); includes insertion of `Option.none` at arbitrary ranks and theorems about the recursion principle |

## Subdirectories

*(No subdirectories)*

## Search Tags

finenum option recursor induction finite-enumeration bijection fin recursion-principle data-transport equivalence
