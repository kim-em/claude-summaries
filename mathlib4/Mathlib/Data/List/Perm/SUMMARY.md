---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/List/Perm
generated: 2025-12-09T10:14:06Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 3
subdirs_count: 0
---

# Perm

## Overview

The `Perm/` subdirectory provides comprehensive theory for list permutations and sub-permutations. It extends the core `List.Perm` relation from Batteries with advanced theorems about permutation equivalence, including interactions with list operations (insertIdx, eraseIdx, foldl, foldr, flatMap, product), relational composition properties, and lattice operations (bagInter). It also defines and develops the sub-permutation relation `Subperm` (`<+~`), which combines subset and permutation properties.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core permutation theory: subset congruence, insertIdx/eraseIdx permutations, relational composition (Perm ∘ Forall₂), fold operations with commutative operators, flatMap/product permutations, and count-based characterizations |
| Lattice.lean | Permutations with lattice operations: bagInter permutations, intersection behavior with append/take/drop/dropSlice, and disjointness properties |
| Subperm.lean | Sub-permutation relation theory: count-based characterization, singleton cases, interaction with cons, and Nodup subset implications |

## Subdirectories

*(none)*

## Search Tags

permutations list-permutations equivalence-relations subpermutations count-invariants fold-operations lattice-operations bag-intersection relational-composition insertIdx eraseIdx flatMap product commutative-operations
