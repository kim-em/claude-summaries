---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/TensorAlgebra
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# TensorAlgebra

## Overview

The `TensorAlgebra/` directory contains the formalization of tensor algebras as the free R-algebra generated R-linearly by a module M. The construction provides the universal property for lifting linear maps from M into R-algebras, establishes that tensor algebras over free modules are themselves free with an explicit basis, shows the graded algebra structure where each grade is a power of the image of the canonical inclusion, and proves the isomorphism between tensor algebras and direct sums of tensor powers. This makes tensor algebras the algebraic counterpart to geometric tensor constructions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core tensor algebra construction: defines TensorAlgebra R M as quotient of FreeAlgebra R M by linearity relations, canonical inclusion ι R : M →ₗ[R] TensorAlgebra R M, lift : (M →ₗ[R] A) ≃ (TensorAlgebra R M →ₐ[R] A) universal property, induction principle, and tprod for constructing products of module elements |
| Basis.lean | Basis theory: equivFreeAlgebra showing tensor algebras over based modules are isomorphic to free algebras, Basis.tensorAlgebra lifting bases on M to FreeMonoid-indexed bases on TensorAlgebra R M, Module.Free instance when M is free, NoZeroDivisors and IsDomain instances, and rank formula as sum of powers of module rank |
| Grading.lean | Graded algebra structure: proves TensorAlgebra R M is ℕ-graded by powers of (ι R).range, auxiliary GradedAlgebra.ι mapping M into graded components, and gradedAlgebra instance showing tensor algebra respects graded multiplication |
| ToTensorPower.lean | Direct sum decomposition: isomorphism equivDirectSum : TensorAlgebra R M ≃ₐ[R] ⨁ n, ⨂[R]^n M, toTensorAlgebra embedding each tensor power into tensor algebra, ofDirectSum and toDirectSum algebra homomorphisms, and proof that product of single-element tensors equals tensor of product |

## Subdirectories

(none)

## Search Tags

tensor-algebra free-algebra universal-property lift basis graded-algebra tensor-power direct-sum module-theory ring-theory multilinear ι tprod rank free-module no-zero-divisors domain
