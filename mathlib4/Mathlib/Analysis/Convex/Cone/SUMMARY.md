---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Convex/Cone
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 6
subdirs_count: 0
---

# Cone

## Overview

The `Cone/` subdirectory contains the topological and analytic theory of convex cones, focusing on results that require topology, norms, or inner products. This extends the purely algebraic theory found in `Mathlib.Geometry.Convex.Cone`. The main topics include proper cones (closed pointed cones), dual cones with respect to continuous bilinear pairings and inner products, Farkas' lemma, the Hahn-Banach separation theorem, M. Riesz extension theorem, and the double dual property that proper cones equal their double dual.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Brief overview explaining this folder covers topological/analytic convex cone theory requiring norms or inner products; lists covered topics including proper cones, dual cones, Farkas' lemma, separation theorems, and M. Riesz extension |
| Basic.lean | Defines proper cones as closed pointed cones (via `ClosedSubmodule`); provides coercions, maps/comaps under continuous linear maps, positive cone construction; proves Farkas' lemma and hyperplane separation for proper cones; establishes double dual property |
| Closure.lean | Defines closure operations for convex cones and pointed cones; provides basic API for closures including coercion and membership lemmas |
| Dual.lean | Defines the dual cone with respect to a continuous perfect bilinear pairing; proves Farkas' lemma for locally convex spaces and hyperplane separation theorem; establishes that the double dual of a proper cone is itself (`dual_dual_flip`, `dual_flip_dual`) |
| Extension.lean | Proves M. Riesz extension theorem: extends linear functionals that are nonnegative on a cone to the whole space while preserving nonnegativity; proves Hahn-Banach theorem for sublinear maps; uses Zorn's lemma for extension construction |
| InnerDual.lean | Specializes dual cone theory to inner product spaces; defines `innerDual` as the cone of points with nonnegative inner product; proves Farkas' lemma for Hilbert spaces, relative hyperplane separation using adjoints, and double inner dual property (`innerDual_innerDual`) |

## Subdirectories

None - this is a leaf directory.

## Search Tags

convex-cones proper-cone dual-cone inner-dual farkas-lemma hyperplane-separation hahn-banach-separation riesz-extension double-dual closed-cone pointed-cone continuous-pairing perfect-pairing inner-product-space hilbert-space locally-convex sublinear-map zorns-lemma functional-analysis separation-theorems
