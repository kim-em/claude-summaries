---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/DirectSum
generated: 2026-01-25T23:20:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# DirectSum

## Overview

The `DirectSum/` directory establishes the relationship between direct sum decompositions and other linear algebra structures. It provides instances showing that direct sums preserve properties like module freeness and finiteness, and develops the critical distributivity relationship between direct sums and tensor products. The main theoretical content shows that tensor products distribute over direct sums (`(⨁ i, M i) ⊗ (⨁ j, N j) ≃ ⨁ (i,j), M i ⊗ N j`), with specialized versions for left/right distribution and interactions with finitely supported functions.

## Key Files

| File | Purpose |
|------|---------|
| Basis.lean | Module.Free instance for direct sums: proves `Module.Free R (⨁ i, M i)` when each component is free, using the equivalence to DFinsupp |
| Finite.lean | Module.Finite instance for finite direct sums: proves `Module.Finite R (⨁ i, M i)` when the index type is finite and each component is finite |
| TensorProduct.lean | Distributivity of tensor products over direct sums: main equivalence `directSum : (⨁ i₁, M₁ i₁) ⊗ (⨁ i₂, M₂ i₂) ≃ ⨁ (i₁,i₂), M₁ i₁ ⊗ M₂ i₂`, unidirectional versions `directSumLeft` and `directSumRight`, and component evaluation lemmas |
| Finsupp.lean | Tensor products with finitely supported functions: linear equivalences `finsuppLeft : (ι →₀ M) ⊗ N ≃ ι →₀ (M ⊗ N)` and `finsuppRight : M ⊗ (ι →₀ N) ≃ ι →₀ (M ⊗ N)`, scalar specializations `finsuppScalarLeft` and `finsuppScalarRight`, and double finsupp tensor product `finsuppTensorFinsupp : (ι →₀ M) ⊗ (κ →₀ N) ≃ (ι × κ) →₀ (M ⊗ N)` with lid/rid variants |

## Subdirectories

(none)

## Search Tags

direct-sum tensor-product finsupp module-free module-finite distributivity linear-equivalence dfinsupp basis finiteness
