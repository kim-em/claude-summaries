---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Lp
generated: 2025-12-05T10:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# Lp

## Overview

The `Lp/` directory provides the theory of L^p norms and spaces in mathlib4. It includes the foundational `WithLp` type synonym for equipping types with L^p norms, implementations of L^p metrics on finite products (`PiLp`) and pairs (`ProdLp`), the full ℓp space of functions with finite p-norm (`lpSpace`), and equivalences among these different L^p constructions. The directory also contains measurable space structures for `WithLp` types and density results showing that smooth compactly supported functions approximate L^p functions.

## Key Files

| File | Purpose |
|------|---------|
| WithLp.lean | Defines the `WithLp p V` type synonym for equipping types with L^p norms; provides canonical inclusions `toLp` and `ofLp` and linear equivalences; serves as the base construction used by `ProdLp` and `PiLp` |
| PiLp.lean | Implements L^p distance on finite products `Π i, α i` where `d(x,y) = (∑ d(xᵢ,yᵢ)^p)^(1/p)` for `0 < p < ∞`, cardinality of non-equal coordinates for `p=0`, and supremum for `p=∞`; provides emetric, metric, normed group and normed space instances; ensures topology is definitionally the product topology |
| ProdLp.lean | Implements L^p distance on binary products `α × β` where `d(x,y) = (d(x₁,y₁)^p + d(x₂,y₂)^p)^(1/p)` for finite `p`; provides parallel structure to `PiLp` but specialized for pairs; straight-forward adaptation of `PiLp.lean` |
| lpSpace.lean | Defines the ℓp space as `lp E p`, the subtype of `Π i, E i` with finite p-norm: finitely supported for `p=0`, `Summable (‖f i‖^p)` for `0 < p < ∞`, or bounded for `p=∞`; equipped with complete normed space structure for `1 ≤ p`; includes Hölder's inequality and norm continuity results |
| LpEquiv.lean | Provides equivalences among L^p spaces: `lpPiLpₗᵢₓ : lp E p ≃ₗᵢ PiLp p E` for `Fintype α`; equivalences between `lp (fun _ ↦ β) ∞` and bounded continuous functions `α →ᵇ β`; includes ring and algebra structure preserving equivalences |
| MeasurableSpace.lean | Defines measurable space structure on `WithLp p X` as the comap of the structure on `X`; proves measurability of `toLp` and `ofLp`; provides `BorelSpace` instances for product and pi types with L^p structure; defines `MeasurableEquiv.toLp` |
| SmoothApprox.lean | Proves density of smooth compactly supported functions in L^p spaces for `p < ∞`; main result `MemLp.exist_sub_eLpNorm_le` shows any L^p function can be approximated by smooth compactly supported functions with arbitrary precision in the L^p norm |

## Subdirectories

(none)

## Search Tags

lp-spaces lp-norms banach-spaces normed-spaces finite-products pi-types product-metrics product-norms with-lp summable-sequences bounded-functions holder-inequality complete-metric-spaces functional-analysis emetric-spaces measurable-structures borel-spaces smooth-approximation compact-support density-results linear-isometric-equivalences

