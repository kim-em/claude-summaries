---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/SkewMonoidAlgebra
generated: 2025-12-04T09:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# SkewMonoidAlgebra

## Overview

This directory implements skew monoid algebras (also called twisted monoid algebras), which generalize the classical monoid algebra construction by incorporating a monoid action on the coefficient ring. Given a monoid G acting on a ring k, the skew monoid algebra is the set of finitely supported functions `G →₀ k` with pointwise addition and a skewed convolution product where `(f * g)(a) = Σ(x*y=a) f(x) * (x • g(y))`. When the action is trivial, this reduces to the standard monoid algebra. The construction is very general, working even when G is merely a magma and k is a not-necessarily-associative semiring, yielding a not-necessarily-unital, not-necessarily-associative algebra.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and structure: `SkewMonoidAlgebra k G` as wrapper around `G →₀ k`, coefficient/support API with extensionality principles, the fundamental skewed convolution product `(f * g)(a) = Σ(x*y=a) f(x) * (x • g(y))`, `single a b` for point masses, semiring/ring/algebra instances with distributivity proofs, module structures over various scalars, `sum` operation for folding over support, natural cast and zero/one elements, equivalence with finsupp via `toFinsuppAddEquiv`, and comprehensive algebraic hierarchy instances (NonUnitalNonAssocSemiring, Ring, CommSemiring, etc.) |
| Lift.lean | Universal properties and homomorphism lifting: `lift k G A : (G →* A) ≃ (AlgHom k (SkewMonoidAlgebra k G) A)` expressing the universal property for algebra homomorphisms, `liftNCAlgHom` for non-commutative lifts when scalar multiplication and ring homomorphism interact properly, `mapDomainAlgHom` for lifting monoid homomorphisms `f : G → H` to algebra homomorphisms between skew monoid algebras, equivalences `equivMapDomain`/`domCongr`/`domLCongr` for transporting along equivalences of the index type, `domCongrAlg` for multiplicative equivalences that respect the action, and `submoduleOfSmulMem` showing k-submodules stable under G-action form SkewMonoidAlgebra-submodules |
| Single.lean | Point modification operations: `erase a f` for zeroing out the coefficient at point a (with support/coefficient interaction lemmas), `update a b` for setting the coefficient at a to b (generalizing both adding and removing elements), induction principle `induction` allowing proofs by building up from single-point functions, decomposition lemma `single_add_erase` showing `single a (f.coeff a) + f.erase a = f`, and update-erase relationship `f.update a b = f.erase a + single a b` |
| Support.lean | Support analysis theorems: support characterization for single elements `support_single_ne_zero`, support bounds for sums `support_sum ⊆ biUnion of component supports`, support of negation `support_neg p = p.support`, support of one element (singleton or subset depending on whether coefficient is nonzero), multiplicative support bounds `support_mul ⊆ f.support * g.support` in pointwise product sense, precise support formulas `support_single_mul_eq_image` and `support_mul_single_eq_image` when multiplication is regular and scalar multiplication is cancellative, and membership characterization `mem_span_support` showing elements lie in the k-span of their support |

## Subdirectories

(none)

## Search Tags

skew-monoid-algebra twisted-monoid-algebra noncommutative-algebra monoid-action convolution-product finitely-supported-functions universal-property lift-homomorphism magma-algebra group-ring semiring-action scalar-tower support-theory single-element coefficient-functions
