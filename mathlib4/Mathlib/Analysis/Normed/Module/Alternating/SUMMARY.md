---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module/Alternating
generated: 2025-12-05T09:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 2
subdirs_count: 1
---

# Alternating

## Overview

The `Alternating/` directory develops the theory of continuous alternating multilinear maps in normed spaces. It defines the operator norm on the space of continuous alternating maps `E [⋀^ι]→L[𝕜] F`, establishing that they form a seminormed (or normed) additive commutative group. The directory provides foundational bounds relating `‖f m‖` to `‖f‖ * ∏ i, ‖m i‖`, proves continuity characterizations, and includes key operations like currying (splitting off the first variable) and uncurrying. Most results are proven by invoking corresponding facts about continuous multilinear maps, since alternating maps are special cases.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core operator norm theory for continuous alternating maps; defines `SeminormedAddCommGroup` and `NormedAddCommGroup` instances for `E [⋀^ι]→L[𝕜] F`; establishes fundamental inequality `‖f m‖ ≤ ‖f‖ * ∏ i, ‖m i‖`; proves continuity characterizations via norm bounds; provides `mkContinuous`, `mkContinuousLinear`, `mkContinuousAlternating` constructors; defines composition operations with linear maps and isometries; includes norm estimates for difference `‖f m₁ - f m₂‖`; shells-based boundedness proofs |
| Curry.lean | Currying operation `curryLeft : E [⋀^Fin (n+1)]→L[𝕜] F → E →L[𝕜] E [⋀^Fin n]→L[𝕜] F`; splits first variable from alternating map to produce continuous linear map into alternating maps; defines `curryLeftLI` as linear isometry; proves norm preservation `‖f.curryLeft‖ = ‖f‖`; establishes interaction with composition operations; shows currying twice with same element gives zero |

## Subdirectories

- [x] `Uncurry/` - Uncurrying operations (`alternatizeUncurryFin` construction, round-trip with curry, second exterior derivative application) (complete)

## Search Tags

alternating-maps continuous-alternating-maps operator-norm multilinear-alternating wedge-product exterior-algebra normed-alternating seminormed-space bounded-alternating mk-continuous currying uncurrying linear-isometry norm-bounds continuity-of-alternating shell-lemma composition-alternating functional-analysis
