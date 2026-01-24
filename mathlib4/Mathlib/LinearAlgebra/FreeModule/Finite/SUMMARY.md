---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/FreeModule/Finite
generated: 2026-01-25T23:51:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Finite

## Overview

The `Finite/` subdirectory develops the theory of finite-rank free modules over rings and principal ideal domains. Core results establish that free modules with finitely-indexed bases are finite (`Module.Finite.of_basis`), and conversely that finite free modules have fintype basis indices. For PIDs, the directory provides quotient decompositions using Smith normal form: submodules of full rank yield quotients isomorphic to products of cyclic modules (quotients by principal ideals). Specialized results for ℤ-modules relate quotient cardinality to determinants of basis changes, compute additive subgroup indices via Smith coefficients, and establish finite quotient characterizations. Linear map modules (M →ₗ[R] N) are shown to be free/finite when M and N are, with explicit rank formulas. Matrix modules and algebra homomorphism spaces receive similar treatment.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Finite free module instances: `Module.Free.ChooseBasisIndex.fintype` (finite modules have fintype basis indices), `Module.Finite.of_basis` (fintype-indexed bases yield finite modules), `Module.Finite.matrix` instance for matrix modules over finite free modules |
| CardQuotient.lean | Cardinality of quotients via determinants for ℤ-modules: `Submodule.natAbs_det_equiv` and `natAbs_det_basis_change` (quotient cardinality equals |det| of basis change matrix), `AddSubgroup.index_eq_natAbs_det` (subgroup index from determinant), `relIndex_eq_natAbs_det` and `relIndex_eq_abs_det` (relative indices via determinants over ℤ and ℚ) |
| Matrix.lean | Linear maps and matrices for finite free modules: `Module.Free.linearMap` and `Module.Finite.linearMap` instances (M →ₗ[R] N is free/finite when M, N are), `Module.finrank_linearMap` (finrank formula: finrank(M →ₗ N) = finrank(M) × finrank(N)), `Finite.algHom` and `card_algHom_le_finrank` (algebra homomorphism finiteness and counting), additive homomorphism instances for ℤ-modules |
| Quotient.lean | Quotient decompositions over PIDs: `quotientEquivPiSpan` (decompose M⧸N as ∏ᵢ R⧸⟨aᵢ⟩ for Smith coefficients aᵢ), `quotientEquivPiZMod` (ℤ-module quotients as ∏ ZMod |aᵢ|), `quotientEquivDirectSum` (direct sum variant), `finiteQuotient_iff` (quotient finite iff submodule has full rank), `finrank_quotient_eq_sum` (dimension formula for quotients) |

## Subdirectories

None.

## Search Tags

finite-free-modules basis fintype smith-normal-form quotient-modules cardinality determinant basis-change subgroup-index principal-ideal-domain PID linear-maps rank-formula matrix-modules algebra-homomorphisms zmod integer-modules direct-sum cyclic-modules
