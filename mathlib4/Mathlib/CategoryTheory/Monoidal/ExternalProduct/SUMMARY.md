---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/ExternalProduct
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# ExternalProduct

## Overview

The `ExternalProduct/` directory formalizes external tensor products for diagrams in monoidal categories. Given two diagrams `K₁ : J₁ ⥤ C` and `K₂ : J₂ ⥤ C` in a monoidal category `C`, the external product `K₁ ⊠ K₂ : J₁ × J₂ ⥤ C` maps each pair `(j₁, j₂)` to the tensor product `K₁ j₁ ⊗ K₂ j₂`. The directory establishes basic properties of this construction including composition laws, braiding isomorphisms, and crucially proves that external products preserve pointwise left Kan extensions when tensor functors preserve appropriate colimits.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines external product bifunctor `⊠` for diagrams in monoidal categories, establishes isomorphisms relating external products to pointwise tensor products via diagonal functors, proves braiding isomorphisms for external products in braided categories, and shows composition compatibility |
| KanExtension.lean | Proves preservation of pointwise left Kan extensions by external products: if `H'` is a pointwise left Kan extension of `H` along `L` and tensoring preserves appropriate colimits, then `H' ⊠ K` (or `K ⊠ H'`) is a pointwise left Kan extension of `H ⊠ K` (or `K ⊠ H`) along the product functor `L.prod (𝟭 E)` (or `(𝟭 E).prod L`) |

## Subdirectories

*(No subdirectories)*

## Search Tags

external-product monoidal-categories tensor-products bifunctors diagram-categories functor-categories pointwise-left-kan-extension colimit-preservation braided-categories natural-isomorphisms currying functor-composition
