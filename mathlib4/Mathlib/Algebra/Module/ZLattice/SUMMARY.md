---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module/ZLattice
generated: 2025-12-01T18:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# ZLattice

## Overview

The `ZLattice/` directory develops the theory of ℤ-lattices in finite-dimensional normed vector spaces over fields like ℝ. A ℤ-lattice is a discrete ℤ-submodule that spans the ambient space over the base field. The directory provides two equivalent perspectives: lattices as spans of bases (`ZSpan` namespace) and lattices as discrete spanning submodules (`IsZLattice` typeclass). It includes fundamental domain theory, covolume computation, lattice index relationships, and convergence results for p-series over lattice points.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core ℤ-lattice definitions and theory: `ZSpan` namespace for lattices as `span ℤ (Set.range b)` with fundamental domains, `fract`/`floor`/`ceil` operations, discrete topology instances; `IsZLattice` typeclass for discrete spanning submodules with freeness/rank theorems, basis conversions `ofZLatticeBasis`, pullback construction `ZLattice.comap` |
| Covolume.lean | Covolume theory for ℤ-lattices: `ZLattice.covolume` as volume of fundamental domain (independent of choice), determinant formula `covolume_eq_det`, lattice index via covolume ratio `covolume_div_covolume_eq_relIndex`, asymptotic point-counting results `tendsto_card_div_pow` and `tendsto_card_le_div` for lattice points in scaled sets |
| Summable.lean | Convergence of power series over lattice points: `summable_norm_rpow` proves `∑ z ∈ L, ‖z‖ʳ` converges for `r < -rank(L)`, `summable_norm_sub_rpow` for shifted series `∑ z ∈ L, ‖z - x‖ʳ`, bound `tsum_norm_rpow_le` via comparison with `∑ k : ℕ, kᵈ⁺ʳ⁻¹`, technical lemmas `normBound` and `abs_repr_lt_of_norm_lt` |

## Subdirectories

*(none)*

## Search Tags

zlattice lattice integer-lattice fundamental-domain discrete-submodule spanning-lattice covolume determinant basis free-module floor-function fract modular-forms number-theory measure-theory fundamental-domain-volume lattice-index p-series convergence summability eisenstein-series norm-bounds

