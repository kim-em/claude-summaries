---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module/Alternating/Uncurry
generated: 2025-12-05T10:15:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Uncurry

## Overview

The `Uncurry/` directory provides the inverse operation to currying for continuous alternating maps. Given a continuous function `f : E →L[𝕜] E [⋀^Fin n]→L[𝕜] F` that is linear in the first argument and alternating in the other `n` arguments, it constructs a continuous alternating form `alternatizeUncurryFin f : E [⋀^Fin (n + 1)]→L[𝕜] F` in `n + 1` arguments via an alternating sum formula. The main round-trip identity shows that uncurrying after currying multiplies the form by `(n + 1)`, which avoids division and works over any normed field. A key application theorem proves that twice uncurrying a symmetric bilinear map yields zero, which will be used to show that the second exterior derivative of differential forms vanishes.

## Key Files

| File | Purpose |
|------|---------|
| Fin.lean | Defines `alternatizeUncurryFin : (E →L[𝕜] E [⋀^Fin n]→L[𝕜] F) → E [⋀^Fin (n + 1)]→L[𝕜] F` via alternating sum `∑ i, (-1)^i • f (v i) (removeNth i v)`; proves round-trip identity `alternatizeUncurryFin (curryLeft f) = (n + 1) • f`; establishes operator norm bound `‖alternatizeUncurryFin f‖ ≤ (n + 1) * ‖f‖`; defines `alternatizeUncurryFinCLM` as continuous linear map with norm `≤ n + 1`; proves `alternatizeUncurryFin_alternatizeUncurryFinCLM_comp_of_symmetric`: twice uncurrying symmetric bilinear maps gives zero; includes application to Fréchet derivatives `fderivCompContinuousLinearMap` composed with symmetric maps; provides technical lemmas `map_insertNth`, `neg_one_pow_smul_map_removeNth_add_eq_zero_of_eq` for alternating sign computations; authored by Yury Kudryashov (2025) |

## Subdirectories

(none)

## Search Tags

alternating-maps continuous-alternating-maps uncurrying alternatizeUncurryFin curry-uncurry-roundtrip operator-norm-bounds exterior-derivative second-derivative-zero symmetric-bilinear differential-forms continuous-linear-map alternating-sum sign-alternation removeNth insertNth multilinear-alternating normed-field frechet-derivative functional-analysis
