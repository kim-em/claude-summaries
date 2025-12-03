---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Ring
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 22
subdirs_count: 2
---

# Ring

## Overview

The `Ring/` directory provides comprehensive theory for ordered rings and semirings, unifying ring-theoretic operations with ordering structures through bundled typeclasses (`OrderedSemiring`, `StrictOrderedSemiring`, `LinearOrderedRing`) and unbundled foundations. The directory spans three conceptual layers: (1) **Foundational unbundled theory** (`Unbundled/`) establishing core lemmas with minimal assumptions and the linear order on rationals; (2) **Algebraic ordering theory** (`Ordering/`) formalizing preorderings and orderings in the classical real algebra sense (Lam 1984), connecting ordered ring structure to quotient constructions via prime ideals; (3) **Comprehensive bundled theory** covering classical results (Bernoulli's inequality, geometric series bounds), specialized structures (nonarchimedean functions, positive cones, archimedean classes), and practical constructions (idempotent Boolean algebras, WithTop/WithBot extensions, various type-preserving operations).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass definitions for ordered (semi)rings: `OrderedSemiring`, `StrictOrderedSemiring`, `OrderedCommSemiring`, `StrictOrderedCommSemiring`, `OrderedRing`, `OrderedCommRing`, `LinearOrderedSemiring`, `LinearOrderedCommSemiring` with interaction axioms between algebraic and order structures |
| Basic.lean | Fundamental lemmas for ordered rings: square nonnegativity (`IsSquare.nonneg`), monoid homomorphism properties (`map_neg_one`, `map_neg`), parity and odd element behavior |
| Canonical.lean | Canonically ordered rings and semirings where addition is canonically ordered: instances for `ZeroLEOneClass`, `MulLeftMono`, `MulRightMono`, and properties of odd elements |
| Abs.lean | Absolute value theory in linearly ordered rings: `abs_mul`, `abs_one`, multiplicative absolute value for zpow (`mabs_zpow`), odd absolute value equivalence |
| Archimedean.lean | Archimedean classes of linearly ordered rings: additive structure on `ArchimedeanClass R` where multiplication becomes addition (`mk x + mk y = mk (x * y)`), preparation for Hahn embedding theorem |
| Cone.lean | Positive cone construction for ordered rings: `RingCone` structure encoding `OrderedRing` and `LinearOrderedRing` axioms via the subset of non-negative elements, bidirectional conversion between cones and ordered rings |
| IsNonarchimedean.lean | Nonarchimedean functions satisfying strong triangle inequality `f(a + b) ≤ max(f a, f b)`: basic properties, interaction with nsmul/nmul, sum bounds for nonnegative functions |
| GeomSum.lean | Geometric series bounds in ordered rings: upper/lower bounds for `∑_{i=0}^{n-1} x^i` and `∑_{i=0}^{n-1} x^i y^{n-1-i}`, positivity results (`geom_sum_pos`), alternating geometric series for `x + 1 ≤ 0` |
| Pow.lean | Bernoulli's inequality and power bounds: standard form `1 + n * a ≤ (1 + a)^n` and generalized form `a^n + n * a^{n-1} * b ≤ (a + b)^n` with various typeclass assumptions |
| Cast.lean | Order properties of integer casts in ordered rings: monotonicity of `Int.cast` (`cast_mono`), characterization of nonnegative casts (`cast_nonneg_iff`), preservation of order relations |
| Idempotent.lean | Boolean algebra structure on idempotent elements in commutative (semi)rings: complement `a ↦ 1 - a`, infimum via multiplication, characterization via pairs `(a,b)` with `a * b = 0` and `a + b = 1` |
| WithTop.lean | Ordered ring structures on `WithTop α`: `instMulZeroClass`, `instOrderedCommSemiring`, multiplication handling infinity (`mul_top'`, `top_mul'`), extending ordered commutative semirings with top element |
| Int.lean | Properties of integers in ordered rings |
| Nat.lean | Properties of natural numbers in ordered rings |
| Rat.lean | Properties of rationals in ordered rings |
| Star.lean | Star operations in ordered rings |
| Units.lean | Units in ordered rings |
| Prod.lean | Product structures for ordered rings |
| Opposite.lean | Opposite ring structures preserving order |
| Synonym.lean | Type synonyms for ordered rings |
| InjSurj.lean | Injectivity and surjectivity lemmas for ordered ring homomorphisms |
| Finset.lean | Finset operations in ordered rings |

## Subdirectories

- [x] `Ordering/` - Classical ring ordering and preordering theory (Lam 1984): subsemirings containing squares but not -1, totality via containment of x or -x, support ideals, and quotient-induced linear orders
- [x] `Unbundled/` - Foundational ordered ring theory using unbundled typeclasses (Semiring + PartialOrder + MulPosMono), including general multiplication monotonicity, sign analysis, AM-GM inequality, and linear order on rationals

## Search Tags

ordered-ring ordered-semiring strict-ordered-ring linear-ordered-ring ordered-comm-ring canonical-ordered-ring ring-cone positive-cone absolute-value bernoulli-inequality geometric-series nonarchimedean archimedean-class idempotent boolean-algebra integer-cast rational-cast with-top with-bot star-ring units product-ring opposite-ring ring-homomorphism
