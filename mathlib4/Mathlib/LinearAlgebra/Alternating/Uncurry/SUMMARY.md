---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Alternating/Uncurry
generated: 2026-01-25T09:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Uncurry

## Overview

The `Uncurry/` directory provides uncurrying operations for alternating maps - the inverse of the currying operations defined in the parent directory. The core construction `alternatizeUncurryFin` takes a function that is linear in the first argument and alternating in `n` remaining arguments, and produces an alternating map in `n+1` arguments via a signed sum formula. The round-trip property `alternatizeUncurryFin (curryLeft f) = (n + 1) • f` shows this is the inverse of currying up to scaling, where the scaling factor is kept to avoid division and work over arbitrary commutative rings.

## Key Files

| File | Purpose |
|------|---------|
| Fin.lean | Defines `alternatizeUncurryFin` which converts `M →ₗ[R] M [⋀^Fin n]→ₗ[R] N` to `M [⋀^Fin (n + 1)]→ₗ[R] N` via signed sum `∑ i, (-1)^i • f (v i) (removeNth i v)`; proves round-trip formula `alternatizeUncurryFin_curryLeft` showing uncurrying after currying gives `(n+1)` times the original; establishes `alternatizeUncurryFin_alternatizeUncurryFinLM_comp_of_symmetric` showing twice-uncurried symmetric bilinear maps vanish (crucial for proving second exterior derivative is zero); includes helper lemmas `map_insertNth` relating insertions to permutation signs and `neg_one_pow_smul_map_removeNth_add_eq_zero_of_eq` for cancellation in alternation proof |

## Subdirectories

None

## Search Tags

alternating-maps uncurrying currying inverse exterior-derivative multilinear-maps signed-sum removeNth insertNth permutation-signs round-trip symmetric-bilinear differential-forms alternatization linear-algebra
