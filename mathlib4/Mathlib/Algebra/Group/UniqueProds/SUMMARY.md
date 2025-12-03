---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/UniqueProds
generated: 2025-12-01T22:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# UniqueProds

## Overview

The `UniqueProds/` directory formalizes the unique products property for multiplicative structures and its additive analogue, unique sums. A group has unique products if any two non-empty finite subsets A, B contain a product element that can be written uniquely as a product of an element from A and an element from B. This property, while uncommon, provides powerful tools for reasoning about monoid algebras and proving zero-divisor-freeness. The directory defines both `UniqueProds` (the existence property) and `TwoUniqueProds` (a stronger property asserting at least two unique pairs exist), proves preservation under equivalences and homomorphisms, and establishes that all ℚ-vector spaces have the unique sums property.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `UniqueMul A B a0 b0` (uniqueness predicate), `UniqueProds G` and `UniqueSums G` typeclasses (existence property for all pairs of finite sets), `TwoUniqueProds`/`TwoUniqueSums` (stronger property with at least two unique pairs); proves closure under products, function types, finsupp; preservation under injective homomorphisms and equivalences; Strojnowski's theorems that groups with `UniqueProds` have `TwoUniqueProds` and that checking `A = B` suffices for cancellative semigroups |
| VectorSpace.lean | Instance showing any ℚ-vector space has `TwoUniqueSums` via basis isomorphism to `Basis.ofVectorSpaceIndex ℚ G →₀ ℚ` and ordered properties of ℚ |

## Subdirectories

(none)

## Search Tags

unique-products unique-sums unique-mul unique-add multiplicative-structures finite-sets monoid-algebra zero-divisors strojnowski vector-space rational-vector-space basis finsupp typeclass homomorphism-preservation equivalence cancellative-semigroup group-property
