---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Star
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Star

## Overview

The `Star/` directory provides the theory of star-ordered rings, algebraic structures where the partial order is characterized by the star operation: `x ≤ y ↔ y = x + p` where `p` is in the additive closure of elements of the form `star s * s`. This framework generalizes C*-algebras and captures the fundamental relationship between order and involution in functional analysis. The directory includes the core `StarOrderedRing` typeclass with two convenient constructors (`of_le_iff`, `of_nonneg_iff`), lemmas about self-adjoint elements, conjugation monotonicity (`star c * a * c`), and instances for product types, Pi types, and natural numbers.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `StarOrderedRing` typeclass defining ordered star rings where `x ≤ y ↔ y = x + p` for `p ∈ closure{star s * s}`, with fundamental lemmas about self-adjoint elements, conjugation, star projections, and instances for ordered modules |
| Conjneg.lean | Order properties of conjugation-negation (`conjneg f`): proves nonnegativity and positivity are preserved under conjugation-negation for functions `G → R` |
| Pi.lean | `StarOrderedRing` instance for Pi types (function spaces) with finite domain, showing product orders respect star structure componentwise |
| Prod.lean | `StarOrderedRing` instance for product types, characterizing the product order via products of closure sets |

## Subdirectories

*(No subdirectories)*

## Search Tags

star-ordered-ring star-algebra c-star-algebra involution self-adjoint conjugation order-theory functional-analysis nonnegative-elements positive-cone star-projection pi-types product-types
