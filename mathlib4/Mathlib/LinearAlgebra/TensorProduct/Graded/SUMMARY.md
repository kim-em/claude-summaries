---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/TensorProduct/Graded
generated: 2026-01-25T09:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Graded

## Overview

The `Graded/` directory implements graded tensor products with signed commutativity for externally and internally graded algebras. The graded tensor product $A \hat\otimes_R B$ features a non-trivial multiplication on homogeneous tensors $(a \otimes b) \cdot (a' \otimes b') = (-1)^{\deg a' \deg b} (a \cdot a') \otimes (b \cdot b')$, generalizing ordinary tensor products with a sign convention essential for super-algebras and graded commutative algebra. This construction supports algebras graded by ℕ, ℤ, ZMod 2, or any index satisfying `Module ι (Additive ℤˣ)`. The directory provides both the fundamental braiding operator (`gradedComm`) implementing signed commutativity and the resulting multiplicative structure, along with a complete universal property characterization.

## Key Files

| File | Purpose |
|------|---------|
| External.lean | Externally-graded tensor products: `gradedComm` (symmetric braiding sending $a \otimes b$ to $(-1)^{\deg a' \deg b} (b \otimes a)$) and `gradedMul` (multiplication for tensor products of direct sum algebras), operating on `(⨁ i, 𝒜 i) ⊗[R] (⨁ i, ℬ i)` with properties including involutivity, compatibility with zero-graded elements, and associativity |
| Internal.lean | Internally-graded tensor products via `GradedAlgebra`: type synonym `GradedTensorProduct R 𝒜 ℬ` (notation `𝒜 ᵍ⊗[R] ℬ`) for `A ⊗[R] B` with graded multiplication, ring/algebra instances, characterization theorem `tmul_coe_mul_coe_tmul` for partially homogeneous elements, inclusion morphisms `includeLeft`/`includeRight`, universal property `liftEquiv` for algebra morphisms with anticommuting homogeneous elements, and symmetric braiding `comm` |

## Subdirectories

None

## Search Tags

graded-tensor-products signed-commutativity super-algebras graded-algebras external-grading internal-grading braiding-operator universal-property anticommutativity direct-sums
