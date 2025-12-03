---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/MonCat
generated: 2025-12-03T00:00:00Z
git_sha: 5bfa1623542d7f245e45ac880c26cfe8f9ecc5ea
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# MonCat

## Overview

The `MonCat/` directory defines the category of monoids and commutative monoids as bundled categorical structures. It introduces four main categories (`MonCat`, `AddMonCat`, `CommMonCat`, `AddCommMonCat`) along with their morphisms (as monoid homomorphisms), forgetful functors, and categorical properties. The directory provides comprehensive categorical infrastructure including limits, colimits, filtered colimits, adjunctions (free-forgetful, adjoin-one-forgetful), corepresentability of forgetful functors, and Yoneda embeddings. This enables treating monoids as objects in a category with full categorical constructions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `MonCat`, `AddMonCat`, `CommMonCat`, `AddCommMonCat` as bundled categories with morphisms as monoid homomorphisms; defines category instances, concrete category structure, forgetful functors between them, universe lift functors, and conversions between isomorphisms and multiplicative equivalences |
| Limits.lean | Proves that monoid categories have all limits and that forgetful functors preserve and create limits; constructs limits as submonoids of sections with small universe conditions |
| Colimits.lean | Constructs all colimits in `MonCat` by building free monoids on prequotients (disjoint unions) modulo monoid relations and diagram morphisms; proves the category has all colimits |
| FilteredColimits.lean | Shows that forgetful functors from monoid categories preserve filtered colimits; constructs monoid structure on filtered colimits in `Type` by passing to common successors |
| Adjunctions.lean | Defines adjunctions: `adjoinOne` functor (adjoining neutral element to semigroups) with forgetful functor to `Semigrp`, and free-forgetful adjunction for monoids (free monoid construction); proves forgetful functors are right adjoints |
| ForgetCorepresentable.lean | Proves forgetful functors are corepresentable: `forget MonCat` is corepresented by `ULift (Multiplicative ℕ)` and `forget AddMonCat` by `ULift ℕ`; establishes natural isomorphisms with coyoneda functors |
| Yoneda.lean | Defines `CommMonCat`-valued coyoneda embeddings and the Hom bifunctor `(Type)ᵒᵖ ⥤ CommMonCat ⥤ CommMonCat` sending `X` and `M` to `X → M` with pointwise operations |

## Subdirectories

(None)

## Search Tags

monoid-categories commutative-monoids bundled-categories category-theory concrete-categories monoid-homomorphisms forgetful-functors limits colimits filtered-colimits adjunctions free-monoid free-forgetful-adjunction corepresentability yoneda-embedding universe-lifting multiplicative-equivalences
