---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module/Alternating
generated: 2025-12-05T10:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 1
---

# Alternating

## Overview

The `Alternating/` directory develops the complete theory of continuous alternating multilinear maps in normed spaces, providing the functional-analytic foundation for exterior algebra and differential forms. It defines the operator norm on the space of continuous alternating maps `E [⋀^ι]→L[𝕜] F`, establishing that they form a seminormed (or normed) additive commutative group with fundamental norm bounds `‖f m‖ ≤ ‖f‖ * ∏ i, ‖m i‖`. The directory implements key structural operations: currying (splitting off the first variable into a linear isometry) and uncurrying (reconstructing alternating maps from curried forms via alternating sums). A central application proves that twice uncurrying symmetric bilinear maps yields zero, establishing the groundwork for showing that the second exterior derivative of differential forms vanishes. Most results are proven by invoking corresponding facts about continuous multilinear maps, since alternating maps are special cases.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core operator norm theory for continuous alternating maps; defines `SeminormedAddCommGroup` and `NormedAddCommGroup` instances for `E [⋀^ι]→L[𝕜] F`; establishes fundamental inequality `‖f m‖ ≤ ‖f‖ * ∏ i, ‖m i‖`; proves continuity characterizations via norm bounds; provides `mkContinuous`, `mkContinuousLinear`, `mkContinuousAlternating` constructors; defines composition operations with linear maps and isometries; includes norm estimates for difference `‖f m₁ - f m₂‖`; shells-based boundedness proofs |
| Curry.lean | Currying operation `curryLeft : E [⋀^Fin (n+1)]→L[𝕜] F → E →L[𝕜] E [⋀^Fin n]→L[𝕜] F`; splits first variable from alternating map to produce continuous linear map into alternating maps; defines `curryLeftLI` as linear isometry; proves norm preservation `‖f.curryLeft‖ = ‖f‖`; establishes interaction with composition operations; shows currying twice with same element gives zero |

## Subdirectories

- [x] `Uncurry/` - Uncurrying operations (`alternatizeUncurryFin` construction, round-trip with curry, second exterior derivative application) (complete)

## Search Tags

alternating-maps continuous-alternating-maps operator-norm multilinear-alternating wedge-product exterior-algebra normed-alternating seminormed-space bounded-alternating mk-continuous currying uncurrying linear-isometry norm-bounds continuity-of-alternating shell-lemma composition-alternating functional-analysis
