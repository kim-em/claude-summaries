---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/CommAlgCat
generated: 2025-12-02T12:00:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# CommAlgCat

## Overview

The `CommAlgCat/` directory defines the bundled category of commutative algebras over a commutative ring `R`, with morphisms as algebra homomorphisms. It establishes the categorical infrastructure including forgetful functors to `CommRingCat` and `AlgCat`, proves equivalence with commutative rings under `R`, and equips the category with co-Cartesian monoidal structure using tensor products. The directory also defines the essentially small subcategory of finitely generated algebras (`FGAlgCat`) and proves essential smallness.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `CommAlgCat R` as bundled category of commutative `R`-algebras; defines morphisms, composition, forgetful functors to `CommRingCat` and `AlgCat`; establishes categorical equivalence with `Under R` (commutative rings under `R`); proves existence of limits and colimits; provides universe lifting functors |
| FiniteType.lean | Defines `FGAlgCat R` as full subcategory of finitely generated `R`-algebras; proves essential smallness by constructing skeleton via multivariate polynomial quotients; provides equivalence with category of finite type ring homomorphisms from `R`; includes universe lifting for finitely generated algebras |
| Monoidal.lean | Establishes monoidal category structure on `CommAlgCat R` using tensor product as monoidal product and `R` as unit; proves associativity, left/right unitors via tensor product algebra equivalences; defines braided structure via commutativity isomorphism; shows opposite category has Cartesian monoidal structure with tensor products as binary products |

## Subdirectories

(none)

## Search Tags

commutative-algebras category-theory bundled-category algebra-morphisms forgetful-functors commutative-rings tensor-product monoidal-category braided-category finitely-generated essentially-small universe-lifting colimits limits cartesian-monoidal finite-type
