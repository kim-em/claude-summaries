---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Algebra/Subalgebra
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 15
subdirs_count: 0
---

# Subalgebra

## Overview

The `Subalgebra/` directory provides comprehensive theory for subalgebras of R-algebras, including their definition, lattice structure, closure operations, maps, and specialized properties. A subalgebra is defined as a subsemiring containing the range of `algebraMap R A`, with complete lattice structure given by the `Algebra.adjoin` operation for taking the minimal subalgebra containing a set. This folder includes operations on subalgebras (products, opposites, centralizers), structural results (tower theory, unitization connections), and technical machinery for working with directed suprema and rank calculations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `Subalgebra R A` structure definition as subsemiring containing `algebraMap` range, with `SetLike` instance, coercion machinery, basic operations (`map`, `comap`, `range`, `inclusion`), and isomorphism theorems |
| Lattice.lean | Complete lattice structure on subalgebras via `Algebra.adjoin` (minimal subalgebra containing a set), Galois connection/insertion between `adjoin` and coercion, and sup/inf operations as adjoin of unions/intersections |
| Centralizer.lean | Centralizer theory for subalgebras including `centralizer_coe_sup` showing centralizer of `S ⊔ T` equals `centralizer S ⊓ centralizer T`, and tensor product results showing centralizers in `A ⊗ B` relate to centers |
| Tower.lean | Subalgebra behavior in algebra towers `A/S/R`, including `IsScalarTower` instances for subalgebras, `restrictScalars` operation to view S-subalgebra as R-subalgebra, and compatibility lemmas |
| Unitization.lean | Connections between non-unital subalgebras and their unitizations, including `NonUnitalSubalgebra.unitization` homomorphism `Unitization R s →ₐ[R] A` with range `Algebra.adjoin R s`, and equivalences when R is a field |
| Operations.lean | Subalgebra-specific versions of ideal operations, including membership criteria for elements via finite sums with powers, and kernel/range results for algebra homomorphisms restricted to subalgebras |
| Pointwise.lean | Pointwise multiplication on subalgebras as submodules, showing `S.toSubmodule * T.toSubmodule ≤ (S ⊔ T).toSubmodule` and equality when the algebra is commutative |
| MulOpposite.lean | Equivalence between subalgebras of `A / R` and `Aᵐᵒᵖ / R` via `Subalgebra.op` and `Subalgebra.unop`, preserving lattice structure |
| Rank.lean | Module rank results for subalgebras using `rank_mul_rank`, including `rank_sup_eq_rank_left_mul_rank_of_free` showing `rank R (A ⊔ B) = rank R A * rank A (adjoin A B)` when modules are free |
| Directed.lean | Directed supremum theory including `coe_iSup_of_directed` showing directed supremum equals union of underlying sets, and `iSupLift` for defining homomorphisms on directed suprema by defining on components |
| IsSimpleOrder.lean | Theorem that finite-dimensional domain algebras over fields with prime dimension have no nontrivial subalgebras (`isSimpleOrder_of_finrank_prime`) |
| Order.lean | Order structure instances (`IsOrderedRing`, `IsStrictOrderedRing`) for subalgebras inheriting from their parent algebra |
| Pi.lean | Product subalgebras `Subalgebra.pi` for dependent products `Π i, S i`, with membership characterized by componentwise containment |
| Prod.lean | Binary product subalgebras `S.prod S₁` as subalgebra of `A × B`, with lattice operations respecting products |
| Pointwise.lean | Additional pointwise operations and idempotency results for subalgebras viewed as submodules |
| Matrix.lean | Matrix subalgebra construction `S.matrix` for square matrices with entries in subalgebra S |

## Subdirectories

*(No subdirectories)*

## Search Tags

subalgebra algebra-closure adjoin lattice-of-subalgebras galois-insertion centralizer algebra-tower restrict-scalars unitization non-unital-subalgebra directed-supremum iSupLift opposite-algebra product-subalgebra rank finite-dimensional simple-order matrix-subalgebra pointwise-operations
