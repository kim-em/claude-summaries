---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/ExteriorPower
generated: 2026-01-25T22:35:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# ExteriorPower

## Overview

This directory formalizes the n-th exterior power `⋀[R]^n M` of a module `M` over a commutative ring `R`, providing both the algebraic construction and its universal property. The exterior power is constructed as a quotient of the exterior algebra, with a canonical alternating map `ιMulti` serving as the universal object. Key results include the universal property (any alternating map factors uniquely through the exterior power), functoriality (linear maps induce maps between exterior powers), and pairings between exterior powers of dual modules and duals of exterior powers.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and universal property: canonical alternating map `ιMulti : M [⋀^Fin n]→ₗ[R] ⋀[R]^n M`, module presentation framework (generators = n-tuples, relations = multilinearity + alternation), universal property as linear equivalence `(M [⋀^Fin n]→ₗ[R] N) ≃ₗ[R] ⋀[R]^n M →ₗ[R] N`, functoriality (`map n f` for linear maps `f`), and natural isomorphisms `⋀[R]^0 M ≃ₗ[R] R` and `⋀[R]^1 M ≃ₗ[R] M` |
| Pairing.lean | Pairing with dual spaces: linear map `toTensorPower` from exterior power to tensor power via alternatization, alternating map `alternatingMapToDual` from dual module to dual of exterior power (determinant formula), canonical pairing `pairingDual : ⋀[R]^n (Module.Dual R M) →ₗ[R] Module.Dual R (⋀[R]^n M)` satisfying `pairingDual (ιMulti f) (ιMulti v) = det (f j (v i))`, and basis duality lemmas for free modules with specified dual pairs |

## Subdirectories

(none)

## Search Tags

exterior-power exterior-algebra alternating-maps multilinear-maps universal-property presentation-theory functoriality dual-pairing determinant tensor-power basis-construction mathlib4 linear-algebra
