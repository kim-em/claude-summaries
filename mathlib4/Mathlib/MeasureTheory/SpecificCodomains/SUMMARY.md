---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/SpecificCodomains
generated: 2026-01-25T21:52:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# SpecificCodomains

## Overview

The `SpecificCodomains/` directory contains specialized results for measurability and integrability of functions valued in specific codomain types. It provides tools for working with integration theory when the target spaces have particular structure: continuous maps on compact spaces (both general continuous maps and those vanishing at a distinguished zero point), product types (Pi types and pairs), and Lp-normed variants of these structures. The main focus is on characterizing when such functions are integrable or belong to Lp spaces, typically by reducing the problem to component-wise conditions.

## Key Files

| File | Purpose |
|------|---------|
| ContinuousMap.lean | Integration theory for `C(Y, E)`-valued functions (continuous maps from compact space Y to normed group E): proves integrability criteria via pointwise bounds, introduces the `mkD` constructor pattern for handling functions that are continuous only almost everywhere, and establishes AE strong measurability for uncurried continuous families |
| ContinuousMapZero.lean | Integration theory for `C(Y, E)₀`-valued functions (continuous maps from compact space Y with distinguished zero to normed group E, vanishing at zero): parallel development to ContinuousMap.lean with additional zero-preservation conditions |
| Pi.lean | Integrability in product spaces: proves that `f : X → Π i, E i` is in Lᵖ if and only if each component `f · i` is in Lᵖ, with analogous results for product types `E × F`, and establishes commutativity of integration with evaluation/projection maps |
| WithLp.lean | Integrability for Lp-normed product types: extends Pi.lean results to `PiLp q E` (dependent products with Lp norm) and `WithLp q (E × F)` (products with Lp norm), proving membership in Lᵖ reduces to component-wise membership, with integral interchange formulas |

## Subdirectories

_(none)_

## Search Tags

integration continuous-map compact-space integrability lp-space product-type pi-type memlp bochner-integral ae-strongly-measurable finite-integral dominated-convergence withlp pilp normed-space banach-space measure-theory specific-codomains
