---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BigOperators/Group/Finset
generated: 2025-12-01T11:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 10
subdirs_count: 0
---

# Finset

## Overview

This folder implements the highest level of the big operator hierarchy: products and sums indexed by finite sets (`Finset`). It defines `Finset.prod` and `Finset.sum` with the standard mathematical notation `∏ i ∈ s, f i` and `∑ i ∈ s, f i`. The implementation builds on `Multiset.prod` by mapping the finset's underlying multiset. Beyond the core definitions and basic theorems, the folder provides specialized lemmas for products and sums over powersets, sigma types, Pi types, integer intervals, and interactions with indicator functions, piecewise functions, and preimages.

## Key Files

| File | Purpose |
|------|---------|
| `Defs.lean` | Core definitions of `Finset.prod` and `Finset.sum`, defined via `(s.1.map f).prod` on the underlying multiset; includes comprehensive notation documentation for bounded operators |
| `Basic.lean` | Fundamental theorems: insertion/deletion lemmas (`prod_insert`, `prod_cons`), singleton/pair products, image products, and other essential properties of finset products |
| `Lemmas.lean` | Miscellaneous lemmas moved from `Basic.lean` to reduce imports: `MonoidHom.finset_prod_apply`, `mulSupport_prod`, `isSquare_prod` |
| `Indicator.lean` | Interaction of big operators with multiplicative/additive indicator functions: `prod_mulIndicator_subset`, `prod_mulIndicator_eq_prod_filter`, `mulIndicator_biUnion` |
| `Piecewise.lean` | Products and sums of piecewise functions including `ite` and `dite`: splitting products over filtered subsets based on predicates |
| `Powerset.lean` | Big operators over powersets: `prod_powerset_insert` (splitting over subsets with/without an element), `prod_powerset`, `prod_powersetCard` |
| `Sigma.lean` | Products over sigma types (`Finset.sigma`): `prod_sigma` converting iterated products over dependent types to single products, `prod_finset_product` for Cartesian products |
| `Pi.lean` | Products over `univ.pi`: equivalence between `univ.pi t` and `Fintype.piFinset t` for dependent function types |
| `Preimage.lean` | Products over preimages: `prod_preimage`, `prod_preimage'`, `prod_preimage_of_bij` for computing products via function preimages |
| `Interval.lean` | Products and sums over integer intervals `Icc`/`Ico`: `prod_Icc_of_even_eq_range` (even functions over symmetric intervals), `prod_Icc_eq_prod_Ico_mul`, `prod_Icc_succ_eq_mul_endpoints` |

## Subdirectories

*(No subdirectories)*

## Search Tags

finset big-operators product sum notation finset-prod finset-sum comm-monoid powerset sigma-type pi-type indicator piecewise preimage interval Icc integer-interval indexed-product indexed-sum
