---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Lie/Derivation
generated: 2025-12-01T11:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Derivation

## Overview

The `Derivation/` directory establishes the theory of Lie derivations on Lie algebras. It defines `LieDerivation` as R-linear maps satisfying the Leibniz rule `D ⁅a, b⁆ = ⁅a, D b⁆ - ⁅b, D a⁆`, develops the algebraic structure (additive group, module, Lie algebra structure on derivations from L to itself), and proves key results connecting derivations to the adjoint action and Killing form. The core result proves that all derivations of finite-dimensional Killing Lie algebras are inner derivations (of the form `ad x` for some `x ∈ L`).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `LieDerivation R L M` as R-linear maps with Leibniz rule `D ⁅a, b⁆ = ⁅a, D b⁆ - ⁅b, D a⁆`; algebraic structure (zero, add, neg, sub, smul, module, Lie algebra on `LieDerivation R L L`); general Leibniz rule `D^[n] ⁅a, b⁆ = Σ choose(n,i) • ⁅D^[i] a, D^[n-i] b⁆`; `inner : M →ₗ[R] LieDerivation R L M` natural map; `exp` automorphism from nilpotent derivations; Noetherian instance for derivations over Noetherian algebras |
| AdjointAction.lean | Adjoint action `ad : L →ₗ⁅R⁆ LieDerivation R L L` as Lie algebra morphism; kernel characterization `ad_ker_eq_center : (ad R L).ker = LieAlgebra.center R L`; injectivity when center is trivial; commutator identity `⁅D, ad x⁆ = ad (D x)`; `ad_isIdealMorphism` proving range of adjoint action is an ideal of derivations |
| Killing.lean | Derivations of finite-dimensional Killing Lie algebras are all inner: `exists_eq_ad` proves `∀ D : LieDerivation R L L, ∃ x, ad R L x = D`; orthogonality properties with respect to Killing form; `range_ad_eq_top` proving adjoint action is surjective onto derivations; Killing form restriction to range of `ad` is nondegenerate |

## Subdirectories

*(none)*

## Search Tags

lie-derivation derivation leibniz-rule adjoint-action inner-derivation killing-form lie-algebra-automorphism nilpotent-derivation exponential center kernel ideal-morphism orthogonal-complement noetherian
