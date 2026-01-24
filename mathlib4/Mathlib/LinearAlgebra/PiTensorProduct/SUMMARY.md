---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/PiTensorProduct
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 5
subdirs_count: 0
---

# PiTensorProduct

## Overview

The `PiTensorProduct/` subdirectory extends the main `PiTensorProduct.lean` file with specialized results about tensor products of indexed families of modules. It provides key distributivity theorems showing that pi tensor products commute with finitely supported functions (`Finsupp`), dependently-typed finitely supported functions (`DFinsupp`), and direct sums (`DirectSum`). The directory also establishes basis theory (constructing a basis for ⨂[R] i, M i from bases of component spaces) and dual space theory (linear equivalences between ⨂[R] i, Dual R (M i) and Dual R (⨂[R] i, M i) for finite free modules).

## Key Files

| File | Purpose |
|------|---------|
| Basis.lean | Basis construction for pi tensor products: `Basis.piTensorProduct` builds a basis for ⨂[R] i, M i from bases b i : κ i → M i, with basis elements ⨂ₜ[R] i, b i (p i) indexed by Π i, κ i |
| DFinsupp.lean | Distributivity over dependent finitely supported functions: `ofDFinsuppEquiv` establishes linear equivalence between ⨂[R] i, (Π₀ j : κ i, M i j) and Π₀ p : Π i, κ i, ⨂[R] i, M i (p i) |
| DirectSum.lean | Distributivity over direct sums: `ofDirectSumEquiv` shows ⨂[R] i, (⨁ j : κ i, M i j) ≃ₗ[R] ⨁ p : Π i, κ i, ⨂[R] i, M i (p i), built from `ofDFinsuppEquiv` |
| Dual.lean | Dual space theory: canonical map `dualDistrib` from ⨂[R] i, Dual R (M i) to Dual R (⨂[R] i, M i), and linear equivalence `dualDistribEquiv` for finite free modules over commutative rings |
| Finsupp.lean | Distributivity over finitely supported functions: `ofFinsuppEquiv` establishes ⨂[R] i, (κ i →₀ M i) ≃ₗ[R] ((i : ι) → κ i) →₀ ⨂[R] i, M i, with variant `ofFinsuppEquiv'` for ground ring modules |

## Subdirectories

(No subdirectories)

## Search Tags

pi-tensor-product indexed-tensor-products basis-construction dual-spaces finsupp dfinsupp direct-sum distributivity multilinear-maps tensor-products linear-equivalence finite-free-modules commutative-rings
