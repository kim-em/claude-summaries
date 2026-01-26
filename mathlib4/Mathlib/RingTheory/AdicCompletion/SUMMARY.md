---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/AdicCompletion
generated: 2026-01-26T20:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# AdicCompletion

## Overview

This directory contains a comprehensive formalization of I-adic completion for modules and rings over a commutative ring R with respect to an ideal I. The theory includes: defining Hausdorff, precomplete, and adic complete modules via convergence of Cauchy sequences modulo I^n • ⊤; constructing the adic completion as an inverse limit of quotients M/(I^n • ⊤); establishing universal properties and functoriality; proving exactness properties over Noetherian rings; showing adic completion as tensor product (proving flatness for Noetherian rings); relating adic completeness to topological properties (complete Hausdorff uniform spaces); and proving structure theorems for complete local rings.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: IsHausdorff, IsPrecomplete, IsAdicComplete classes; AdicCompletion construction as inverse limit; Hausdorffification; universal property via lift; characterizations of injectivity/surjectivity/bijectivity of canonical map |
| Algebra.lean | Algebra structure on adic completions: commutative ring instance on AdicCompletion I R; module structure AdicCompletion I M over AdicCompletion I R; evalₐ algebra map to quotients R/(I^n); liftRingHom and liftAlgHom for compatible families of maps |
| AsTensorProduct.lean | Identifies adic completion with tensor product: natural map AdicCompletion I R ⊗[R] M → AdicCompletion I M; proves bijection for M = R^n (finite type); surjectivity for finite modules; bijection for finite modules over Noetherian rings; flatness of adic completion over Noetherian rings |
| Exactness.lean | Exactness properties of adic completion functors: map_surjective (preserves surjectivity); map_injective (preserves injectivity on finite modules over Noetherian rings); map_exact (exact functor on finite modules over Noetherian rings) |
| Functoriality.lean | Functorial properties and finite product/sum behavior: LinearMap.map inducing functorial maps on completions; commutation with finite sums (sumEquivOfFintype); commutation with finite products (piEquivOfFintype); surjectivity criteria via quotient maps |
| LocalRing.lean | Complete local rings: proves that I-adic complete ring with maximal ideal I is a local ring; characterizes units as elements not in maximal ideal (isUnit_iff_notMem_of_isAdicComplete_maximal) |
| Noetherian.lean | Hausdorff properties for Noetherian modules: automatic Hausdorff for ideals in Jacobson radical over Noetherian rings; Hausdorff for local rings; Hausdorff for torsion-free modules over domains |
| RingHom.lean | Lifting ring homomorphisms to completions: IsAdicComplete.liftRingHom for compatible families of maps to quotients; IsAdicComplete.liftAlgHom for algebra homomorphism version; universal property and uniqueness theorems; variants for strictly monotone sequences |
| Topology.lean | Connection between adic and topological properties: IsHausdorff I R ↔ T2Space R in adic topology; IsPrecomplete I R ↔ CompleteSpace R in adic topology; IsAdicComplete I R ↔ CompleteSpace R ∧ T2Space R |

## Subdirectories

(none)

## Search Tags

adic-completion completion Hausdorff precomplete adic-complete Cauchy-sequence inverse-limit I-adic topology uniform-space tensor-product flatness exactness functoriality local-ring Noetherian Jacobson-radical universal-property lift module-theory commutative-algebra
