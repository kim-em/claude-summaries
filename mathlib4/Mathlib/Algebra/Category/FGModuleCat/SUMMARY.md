---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/FGModuleCat
generated: 2025-12-02T16:30:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# FGModuleCat

## Overview

The `FGModuleCat/` directory defines the category of finitely generated modules over a ring `R`, implemented as a full subcategory of `ModuleCat R`. When `R` is a field, this specializes to finite-dimensional vector spaces. The directory provides categorical infrastructure including monoidal structure (when `R` is commutative), closed monoidal structure (when `R` is a field), right-rigid structure with duality, limits and colimits, abelian category structure (when `R` is Noetherian), and a proof of essential smallness.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `FGModuleCat R` as full subcategory of finitely generated modules; includes monoidal structure for commutative rings, closed monoidal and right-rigid structures for fields, duality with evaluation/coevaluation maps, universe lifting functor |
| Limits.lean | Proves `FGModuleCat k` (over Noetherian ring `k`) has all finite limits via forgetful functor to `ModuleCat k` creating limits; limits realized as subobjects of finite products |
| Colimits.lean | Proves `FGModuleCat k` has all finite colimits via forgetful functor to `ModuleCat k` creating colimits; colimits realized as quotients of finite coproducts |
| Abelian.lean | Proves `FGModuleCat k` is an abelian category when `k` is a Noetherian ring, by showing coimage-image comparison is always an isomorphism |
| EssentiallySmall.lean | Proves `FGModuleCat R` is essentially small by providing explicit small model `FGModuleRepr R` representing modules as quotients of `R^n` by submodules; includes equivalence between small model and standard category |

## Subdirectories

None.

## Search Tags

finitely-generated-modules category-theory monoidal-category closed-monoidal rigid-category duality vector-spaces finite-dimensional limits colimits abelian-category noetherian essentially-small universe-lifting evaluation coevaluation
