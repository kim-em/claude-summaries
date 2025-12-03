---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/Ring/Under
generated: 2025-12-03T11:00:00Z
git_sha: 5bfa1623542d7f245e45ac880c26cfe8f9ecc5ea
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Under

## Overview

The `Under/` directory provides the API for working with the comma category `Under R` for commutative rings `R : CommRingCat`, which is equivalent to the category of commutative `R`-algebras. It establishes the connection between categorical morphisms in `Under R` and algebra homomorphisms, provides functorial constructions like base change via tensor products, and proves preservation properties for limits under flatness assumptions. This framework allows working with `R`-algebras categorically while maintaining compatibility with the algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core API for `Under R`: coercion to types, algebra instances, conversion between `Under R` morphisms and algebra homomorphisms (`toAlgHom`, `AlgHom.toUnder`, `AlgEquiv.toUnder`), constructor `mkUnder`, base change functor `tensorProd R S` (mapping `A ↦ S ⊗[R] A`), and natural isomorphism showing tensor product equals pushout |
| Limits.lean | Limit constructions in `Under R`: canonical product fans using Pi types, equalizer forks using `AlgHom.equalizer`, proves `tensorProd R S` preserves finite products and finite limits when `S` is `R`-flat, establishes that `Under.pushout f` is left-exact (preserves finite limits) when `f` is flat |

## Subdirectories

*(None)*

## Search Tags

category-theory commutative-algebras comma-categories under-category algebra-homomorphisms tensor-products base-change functors limits products equalizers flat-modules pushouts left-exactness R-algebras algebraic-structures categorical-algebra
