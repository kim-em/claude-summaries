---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module/Multilinear
generated: 2025-12-05T09:15:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Multilinear

## Overview

The `Multilinear/` directory provides the theory of continuous multilinear maps in normed spaces with operator norm. It defines the operator norm `‖f‖` as the smallest number satisfying `‖f m‖ ≤ ‖f‖ * ∏ i, ‖m i‖` for all inputs, proves this defines a normed space structure on `ContinuousMultilinearMap 𝕜 E G`, and establishes the equivalence between continuity and boundedness. The directory also provides currying/uncurrying operations that transform multilinear maps in `n+1` variables into linear maps to multilinear maps in `n` variables, with corresponding linear isometric equivalences.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Operator norm theory for continuous multilinear maps: defines `‖f‖` as inf of bounds `C` satisfying `‖f m‖ ≤ C * ∏ i, ‖m i‖`; proves equivalence `continuous ↔ bounded` via `exists_bound_of_continuous` and `continuous_of_bound`; establishes fundamental inequality `le_opNorm`; provides difference bounds `norm_image_sub_le`; constructs `mkContinuous` to promote bounded multilinear maps to continuous ones; proves normed space structure including completeness, metric properties, composition operations |
| Curry.lean | Currying and uncurrying for continuous multilinear maps: `curryLeft` converts `n+1`-variable multilinear map to linear map into `n`-variable multilinear maps by separating first variable; `curryRight` separates last variable; `curryMid` separates arbitrary variable; provides inverse operations `uncurryLeft`, `uncurryRight`, `uncurryMid`; establishes linear isometric equivalences `continuousMultilinearCurryLeftEquiv`, `continuousMultilinearCurryRightEquiv`, `continuousMultilinearCurryMidEquiv`; proves norm preservation and boundedness under currying transformations |

## Subdirectories

No subdirectories.

## Search Tags

continuous-multilinear-maps operator-norm bounded-multilinear normed-spaces currying uncurrying linear-isometry multilinear-algebra functional-analysis norm-bounds continuity-boundedness mkContinuous opNorm product-norms fin-indexed curry-left curry-right curry-mid linear-equiv isometry seminormed-spaces
