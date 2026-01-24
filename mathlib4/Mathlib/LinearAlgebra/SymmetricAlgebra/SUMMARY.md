---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/SymmetricAlgebra
generated: 2026-01-25T10:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# SymmetricAlgebra

## Overview

The `SymmetricAlgebra/` directory formalizes the symmetric algebra construction, which builds the free commutative R-algebra generated R-linearly by a module M. The symmetric algebra is constructed as a quotient of the tensor algebra by the commutativity relation, making elements commute. This provides the algebraic counterpart to symmetric tensors, with canonical applications to polynomial algebras (the symmetric algebra of a free module is isomorphic to multivariate polynomials over its basis). The directory includes the core construction with universal property and basis theory connecting to multivariate polynomials.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core symmetric algebra construction: concrete definition as quotient `RingQuot (SymRel R M)` of tensor algebra by commutativity relation `ι R x * ι R y ∼ ι R y * ι R x`, commutative semiring and commutative ring instances, canonical inclusion `ι : M →ₗ[R] SymmetricAlgebra R M`, universal property via `lift : (M →ₗ[R] A) ≃ (SymmetricAlgebra R M →ₐ[R] A)` for commutative R-algebras A, and `IsSymmetricAlgebra` predicate characterizing algebras satisfying the universal property |
| Basis.lean | Basis theory for symmetric algebras: isomorphism `equivMvPolynomial b : SymmetricAlgebra R M ≃ₐ[R] MvPolynomial I R` given basis `b : Basis I R M`, lifting basis to symmetric algebra via `Basis.symmetricAlgebra b : Basis (I →₀ ℕ) R (SymmetricAlgebra R M)`, freeness instance `instModuleFree` when M is free, no-zero-divisors and domain instances for free modules over integral domains, and rank formula `rank R (SymmetricAlgebra R M) = max (rank R M) ℵ₀` for nontrivial free modules |

## Subdirectories

(none)

## Search Tags

symmetric-algebra tensor-algebra quotient-algebra commutative-algebra free-algebra universal-property multivariate-polynomials basis free-modules rank commutativity-relation polynomial-algebras symmetric-tensors
