---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/IntegralClosure/Algebra
generated: 2026-02-01T19:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 3
subdirs_count: 0
---

# Algebra

## Overview

The `Algebra/` directory defines and develops the theory of integral algebras. An algebra `A` over `R` is integral if every element of `A` is integral over `R`. The main type class `Algebra.IsIntegral R A` captures this property. This directory also defines `integralClosure R A`, the subalgebra of `A` consisting of all elements integral over `R`, and proves it is closed under algebraic operations. Additionally, it develops the theory of integrality over ideals, showing that elements in the image of an ideal under an integral extension satisfy monic polynomials with coefficients controlled by powers of the ideal.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines the type class `Algebra.IsIntegral R A` (all elements of A are integral over R) and provides the `isIntegral_def` characterization; minimal dependencies |
| Basic.lean | Main development: proves integral elements form a subalgebra (`integralClosure R A`), integrality is preserved under algebra homomorphisms (surjective, injective, equivalences), finite modules are integral (`IsIntegral.of_finite`), integral algebras closed under products and tensor products, and `MulSemiringAction` on integral closures |
| Ideal.lean | Integrality over ideals: proves that elements in `I.map (algebraMap R S)` for an integral extension satisfy monic polynomials whose coefficients lie in appropriate powers of `I` (Stacks 00H5); key lemma shows the `X^{n-i}` coefficient lies in `I^{n-i}` |

## Subdirectories

(none)

## Search Tags

Algebra.IsIntegral integral-algebra integralClosure subalgebra IsIntegral.of_finite Module.Finite integral-element monic-polynomial integral-closure algebra-homomorphism tensor-product integrality-over-ideals ideal-map Stacks-00H5 Stacks-00GK RingHom.Finite MulSemiringAction
