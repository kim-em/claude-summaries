---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Tropical
generated: 2025-12-04T07:15:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Tropical

## Overview

The `Tropical/` directory implements tropical algebra, a mathematical structure where ordinary addition is replaced by minimum (or maximum) and ordinary multiplication is replaced by addition. This provides a complete semiring structure for min-plus algebra (with max-plus as the dual via `OrderDual`). The implementation uses a type synonym `Tropical R` that reinterprets operations on the underlying type `R`, establishing tropical addition as `min`, tropical multiplication as `+`, tropical zero as `⊤`, and tropical one as `0`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core tropical algebra definitions: `Tropical R` type synonym with conversion functions (`trop`/`untrop`), tropical addition as minimum (`x + y = min x y`), tropical multiplication as underlying addition, algebraic hierarchy from semigroups up to `CommSemiring (Tropical R)` for linearly ordered types with top, equivalences and order isomorphisms, and no-zero-divisors property for `Tropical (WithTop R)` |
| BigOperators.lean | Tropicalization of finitary operations converting between sums/products and infima: key results `trop (∑ i, f i) = ∏ i, trop (f i)` and `untrop (∏ i, f i) = ∑ i, untrop (f i)` for finite sums/products, conversions between infima and sums (`trop (s.inf f) = ∑ i ∈ s, trop (f i)`), and results for conditionally complete lattices relating tropical sums to infima over finsets/fintypes, enabling expression of tropical polynomial evaluation as minima over piecewise linear functions |
| Lattice.lean | Order structures on tropical types: defines `ConditionallyCompleteLattice (Tropical R)` and `ConditionallyCompleteLinearOrder (Tropical R)` instances that lift the underlying lattice structure of `R` through the tropical isomorphism, with semilattice instances for inf/sup operations preserving the definitional order equality |

## Subdirectories

(none)

## Search Tags

tropical algebra min-plus max-plus semiring idempotent linear-order lattice big-operators infimum supremum tropical-geometry type-synonym order-isomorphism
