---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Hall
generated: 2025-12-08T07:42:05Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Hall

## Overview

This directory contains the formalization of **Hall's Marriage Theorem** in two versions: a finite case requiring the index type to be finite (`Finite.lean`), and a generalized case using a compactness argument to remove the finiteness constraint (`Basic.lean`). The theorem states that for an indexed family of finite sets, there exists a system of distinct representatives (an injective function selecting one element from each set) if and only if every union of k sets contains at least k elements (the Hall condition).

## Key Files

| File | Purpose |
|------|---------|
| Finite.lean | Hall's Marriage Theorem for finite index types `ι`: proves `Finset.all_card_le_biUnion_card_iff_existsInjective'` using strong induction with two cases (strict inequality vs. tight equality for some subset), serving as the base case for the generalized theorem |
| Basic.lean | Generalized Hall's Marriage Theorem removing the `Fintype ι` constraint: uses inverse limit compactness (`nonempty_sections_of_finite_inverse_system` from Tychonoff) to bootstrap from the finite case; provides three formulations in terms of `Finset`, relations `SetRel α β`, and `Finset.filter` |

## Subdirectories

None.

## Search Tags

hall-marriage-theorem matching system-of-distinct-representatives hall-condition transversal injective-function indexed-families finite-sets compactness inverse-limit tychonoff bipartite-matching combinatorics
