---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/CopyDiscardCategory
generated: 2025-12-07T08:35:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# CopyDiscardCategory

## Overview

The `CopyDiscardCategory/` directory formalizes copy-discard categories, which are symmetric monoidal categories where every object has a compatible commutative comonoid structure. These categories arise in the categorical semantics of probabilistic programming and quantum mechanics, where copy and discard operations represent cloning and deletion. The formalization includes the basic theory of copy-discard categories, deterministic morphisms (those that preserve copy operations), and the important special case showing that cartesian monoidal categories are copy-discard categories where copy is the diagonal and discard is the unique map to terminal.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `CopyDiscardCategory` class with copy (Δ) and discard (ε) operations satisfying tensor compatibility axioms |
| Deterministic.lean | Defines `Deterministic` morphisms that preserve copy operations (alias for comonoid homomorphisms) |
| Cartesian.lean | Shows every cartesian monoidal category is a copy-discard category with all morphisms deterministic |

## Subdirectories

*(No subdirectories)*

## Search Tags

copy-discard-category comonoid symmetric-monoidal cartesian deterministic-morphisms probabilistic-programming categorical-semantics diagonal-map
