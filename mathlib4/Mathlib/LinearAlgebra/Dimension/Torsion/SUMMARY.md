---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Dimension/Torsion
generated: 2026-01-25T17:08:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Torsion

## Overview

The `Torsion/` subdirectory establishes fundamental relationships between module rank (dimension) and torsion elements in modules over commutative rings. The central results show that torsion submodules don't contribute to rank: quotients by torsion submodules preserve rank (`rank M/N = rank M` when `N ≤ torsion M`), and modules have rank zero if and only if they are entirely torsion (`rank M = 0 ↔ Module.IsTorsion M` over integral domains). These results connect the cardinal-valued dimension theory from the parent directory with the algebraic notion of torsion from `Mathlib.Algebra.Module.Torsion`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Proves `rank_quotient_eq_of_le_torsion`: quotients by torsion submodules preserve rank, establishing that torsion elements don't contribute to module dimension |
| Finite.lean | Characterizes zero-dimensional modules via torsion: `rank_eq_zero_iff_isTorsion` (rank zero iff entirely torsion over domains) and `finrank_eq_zero_iff_isTorsion` (finite rank version requiring StrongRankCondition) |

## Subdirectories

None

## Search Tags

torsion rank dimension module quotient torsion-submodule rank-zero integral-domain commutative-ring finrank strong-rank-condition linear-independence
