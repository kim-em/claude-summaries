---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Central
generated: 2025-12-04T15:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Central

## Overview

The `Central/` directory contains the theory of central algebras over commutative rings. A central algebra `D` over a commutative ring `K` is one where the center of `D` (elements that commute with everything) is exactly the image of `K` in `D`. This concept is fundamental in noncommutative algebra, particularly for central simple algebras (CSAs) over fields, which play a key role in the Brauer group and division algebra theory. The directory includes both the core definitions and results about how centrality behaves under standard algebraic constructions like tensor products, matrix algebras, and endomorphism algebras.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines the `Algebra.IsCentral K D` typeclass requiring `Subalgebra.center K D ≤ ⊥`, with extensive documentation on central simple algebras and implementation notes on typeclass design |
| Basic.lean | Core results: `center_eq_bot`, `mem_center_iff`, `self` instance (commutative rings are central over themselves), `baseField_essentially_unique` (field extension uniqueness), `of_algEquiv` (centrality under isomorphism), and opposite algebra instance |
| End.lean | Proves that endomorphism algebras `Module.End R M` on free modules are central algebras over `R` |
| Matrix.lean | Proves that matrix algebras `Matrix n n D` are central over `K` when `D` is central over `K`, using the characterization that the center equals scalar matrices |
| TensorProduct.lean | Tensor product theory: proves that if `B ⊗[K] C` is central and nontrivial over a field `K`, then both `B` and `C` must be central algebras (with variants for general commutative base with flatness/injectivity conditions) |

## Subdirectories

*(none)*

## Search Tags

central-algebra center noncommutative-algebra central-simple-algebra tensor-product matrix-algebra endomorphism-algebra brauer-group division-algebra field-theory
