---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/ContMDiff
generated: 2026-01-24T07:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# ContMDiff

## Overview

The `ContMDiff/` directory contains the core definitions and foundational properties of continuously differentiable maps (`C^n` functions) between smooth manifolds in Mathlib. This is the central API for manifold smoothness, defining the predicates `ContMDiff`, `ContMDiffAt`, `ContMDiffOn`, and `ContMDiffWithinAt` that characterize when a function between manifolds is `n` times continuously differentiable. The implementation leverages the local invariant properties framework to lift smoothness from model spaces to manifolds, ensuring coordinate-independence. The smoothness index `n` can be a natural number, `infinity` (smooth), or `omega` (analytic).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of `ContMDiff`, `ContMDiffAt`, `ContMDiffOn`, `ContMDiffWithinAt`; characterizations via extended charts; equivalence results between different formulations; restriction and congruence lemmas; locality of smoothness |
| Basic.lean | Fundamental properties: composition (`ContMDiffOn.comp`, `ContMDiff.comp`), identity (`contMDiff_id`), constants (`contMDiff_const`), iteration, inclusion maps between open sets, open embeddings, piecewise functions, and testing smoothness on unions of open sets |
| Atlas.lean | Smoothness of atlas members and local structomorphisms; model with corners is smooth; charts and extended charts are smooth on their domains; elements of `contDiffGroupoid` are smooth; characterization of local structomorphisms via bi-directional smoothness |
| Constructions.lean | Smoothness of product and sum constructions: `Prod.mk`, `Prod.fst`, `Prod.snd`, `Prod.map`, `Sum.inl`, `Sum.inr`, `Sum.elim`, `Sum.map`, `Sum.swap`; currying lemmas; functions into pi types; composition lemmas for two-argument functions |
| NormedSpace.lean | Equivalence between manifold-smoothness and usual smoothness for functions between vector spaces (`contMDiff_iff_contDiff`); continuous linear maps are smooth; smoothness of `clm_comp`, `clm_apply`, `clm_prodMap`, `cle_arrowCongr`; scalar multiplication is smooth |

## Subdirectories

(none)

## Search Tags

contmdiff contmdiffat contmdiffon contmdiffwithinat smooth-map c-n-function manifold-smoothness chart-smoothness atlas-smoothness composition-smoothness product-manifold sum-manifold linear-map-smooth scalar-multiplication local-structomorphism extended-chart
