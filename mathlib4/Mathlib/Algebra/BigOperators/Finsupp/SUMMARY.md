---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BigOperators/Finsupp
generated: 2025-12-01T10:35:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Finsupp

## Overview

The `Finsupp/` directory provides comprehensive infrastructure for big operators (sums and products) over finitely-supported functions (`Finsupp`). It defines `Finsupp.sum` and `Finsupp.prod` which iterate over the support of a finsupp, along with extensive API for manipulating these operations including index transformations, homomorphism properties, and specialized results for `Fin` types. The theory connects finsupps with big operators through canonical isomorphisms like `liftAddHom` and covers operations like addition index manipulation, embedding domains, and indicator functions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of `Finsupp.sum` and `Finsupp.prod`: defines `f.prod g = ∏ a ∈ f.support, g a (f a)`, includes index manipulation (`prod_add_index`, `prod_mapRange_index`), homomorphism properties (`map_finsuppProd`), canonical isomorphism `liftAddHom : (α → M →+ N) ≃+ ((α →₀ M) →+ N)`, and specialized results for single elements, indicator functions, and finset sums |
| Fin.lean | Big operators for finsupps over `Fin` types: `sum_cons` and `sum_cons'` for decomposing sums over `Fin (n+1)` into head and tail, equivalence `finTwoArrowEquiv' : (Fin 2 →₀ M) ≃ M × M` with sum formula showing `((finTwoArrowEquiv' M).symm d).sum = d.1 + d.2` |

## Subdirectories

(none)

## Search Tags

finsupp finitely-supported-functions big-operators sum product support index-transformation homomorphism liftAddHom single indicator embedding fin equivalence additive-homomorphism multiplicative-homomorphism
