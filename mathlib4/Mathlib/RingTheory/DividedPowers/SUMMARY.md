---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/DividedPowers
generated: 2026-01-26T20:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# DividedPowers

## Overview

The `DividedPowers/` directory formalizes divided power structures on ideals in commutative rings, a fundamental construction in crystalline cohomology and p-adic geometry. A divided power structure on an ideal I provides operations dpow(n, a) modeling the intuitive formula a^n/n!, satisfying axioms that generalize binomial theorem properties without requiring divisibility by factorials. The directory provides the core definition and axioms, constructions for specific rings (ℚ-algebras, p-adic integers, square-zero ideals, characteristic p rings), morphisms between divided power structures, and the theory of sub-dp-ideals (subideals preserved by divided powers).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of divided power structures on ideals; axioms (dpow_null, dpow_zero, dpow_one, dpow_add, dpow_mul, mul_dpow, dpow_comp); basic lemmas including exponential series, factorial formula, nilpotency, and product/sum formulas; transfer via ring equivalences |
| DPMorphism.lean | Divided power morphisms between ideals with DP structures; unbundled IsDPMorphism and bundled DPMorphism; construction fromGens for morphisms compatible on generating sets; composition of DP morphisms; uniqueness theorem dpow_eq_from_gens showing DP structures determined by values on generators |
| RatAlgebra.lean | Examples of divided power structures via x^n/n!; OfInvertibleFactorial construction when (n-1)! is invertible and I^n = 0; OfSquareZero for square-zero ideals; CharP for characteristic p rings with I^p = 0; RatAlgebra construction for ℚ-algebras with uniqueness theorem showing it's the only possible DP structure |
| Padic.lean | Divided power structure on (p) ⊆ ℤ_[p] constructed via dpow n x = x^n/n!; uses ofInjective to lift DP structure from ℚ_[p] to ℤ_[p]; proves norm bounds showing dpow preserves p-adic valuation; coe_dpow_eq formula for coercion to ℚ_[p] |
| SubDPIdeal.lean | Theory of sub-dp-ideals (subideals J ⊆ I where dpow(n, j) ∈ J for j ∈ J); bundled SubDPIdeal and unbundled IsSubDPIdeal; induced DP structures on sub-dp-ideals; quotient DP structures when ker(f) ∩ I is sub-dp-ideal; complete lattice structure on sub-dp-ideals; span construction and characterization theorems |

## Subdirectories

(none)

## Search Tags

divided-powers crystalline-cohomology p-adic commutative-algebra ideal dpow factorial binomial nilpotent exponential-series dp-morphism sub-dp-ideal quotient ring-equivalence rat-algebra padic-integers square-zero characteristic-p Berthelot Roby Ogus uniformBell multinomial
