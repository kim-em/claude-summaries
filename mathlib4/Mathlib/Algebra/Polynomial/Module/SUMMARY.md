---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Polynomial/Module
generated: 2025-12-01T10:40:15Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Module

## Overview

The `Module/` directory provides `R[X]`-module structures on `R`-modules, offering two complementary constructions: `Module.AEval R M a` which turns an `R`-module `M` into an `R[X]`-module via evaluation at an algebra element `a`, and `PolynomialModule R M` which constructs the polynomial module `M[X]` as a type alias for `ℕ →₀ M`. These structures enable treating modules as polynomial modules with polynomial scalar multiplication, connecting polynomial algebra with module theory and providing tools for studying endomorphisms and tensor products.

## Key Files

| File | Purpose |
|------|---------|
| AEval.lean | Defines `Module.AEval R M a`: `R[X]`-module structure on `M` where polynomial `f` acts via `f • m = aeval a f • m`, with abbreviation `Module.AEval' φ` for linear endomorphisms, order isomorphism between invariant submodules and `R[X]`-submodules, and annihilator theory |
| Basic.lean | Defines `PolynomialModule R M := ℕ →₀ M`: the `R[X]`-module `M[X]`, with monomial construction `single`/`lsingle`, polynomial scalar multiplication via `aeval`, evaluation `eval r : M[X] →ₗ[R] M`, composition `comp p : M[X] →ₗ[R] M[X]`, and isomorphisms `equivPolynomialSelf : R[X] ≃ₗ[R[X]] R[X]` and `equivPolynomial : S[X] ≃ₗ[R] S[X]` |
| FiniteDimensional.lean | Proves torsion results for finite-dimensional polynomial modules: `isTorsion_of_aeval_eq_zero` (polynomial annihilation implies torsion) and `isTorsion_of_finiteDimensional` (finite-dimensional algebra implies induced `K[X]`-module is torsion via minimal polynomial) |
| TensorProduct.lean | Establishes `R[X]`-linear isomorphism `polynomialTensorProductLEquivPolynomialModule : R[X] ⊗[R] M ≃ₗ[R[X]] PolynomialModule R M`, connecting tensor product and polynomial module structures |

## Subdirectories

*(No subdirectories)*

## Search Tags

polynomial-module module-structure aeval polynomial-action scalar-multiplication invariant-submodule annihilator torsion-module finite-dimensional minimal-polynomial tensor-product endomorphism evaluation composition
