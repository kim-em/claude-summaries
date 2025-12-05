---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module/PiTensorProduct
generated: 2025-12-05T08:45:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# PiTensorProduct

## Overview

This directory defines two fundamental seminorms on pi-type tensor products `⨂[𝕜] i, Eᵢ` of finite families of normed spaces. The projective seminorm provides an upper bound on all norms satisfying the basic tensor product inequality, while the injective seminorm characterizes the universal property for continuous multilinear maps. Together, these establish the normed space structure on tensor products and prove the isometric linear equivalence between continuous multilinear maps and continuous linear maps out of the tensor product.

## Key Files

| File | Purpose |
|------|---------|
| ProjectiveSeminorm.lean | Defines the projective seminorm as the infimum over all representations `x = ∑ⱼ ⨂ₜ[𝕜] mⱼ i` of `∑ⱼ ∏ᵢ ‖mⱼ i‖`; proves `‖f.lift x‖ ≤ projectiveSeminorm x * ‖f‖` for continuous multilinear maps; provides upper bound for all reasonable tensor product norms |
| InjectiveSeminorm.lean | Defines the injective seminorm as `sup` over dual embeddings into operator norm spaces; establishes the universal property `ContinuousMultilinearMap 𝕜 E F ≃ₗᵢ[𝕜] (⨂[𝕜] i, Eᵢ) →L[𝕜] F` as isometric linear equivalence; defines functorial operations `mapL`, `tprodL`, and `mapLMultilinear`; proves `‖PiTensorProduct.mapL f‖ ≤ ∏ i, ‖fᵢ‖` |

## Subdirectories

None.

## Search Tags

tensor-products pi-tensor-product projective-seminorm injective-seminorm multilinear-maps continuous-multilinear-maps universal-property isometric-equivalence operator-norm functoriality lift normed-spaces seminorms finite-families
