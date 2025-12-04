---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/IdealSheaf
generated: 2025-12-04T21:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# IdealSheaf

## Overview

The `IdealSheaf/` directory provides a comprehensive formalization of ideal sheaves on schemes in algebraic geometry. It defines the structure `IdealSheafData` containing the data to uniquely define an ideal sheaf (ideals on affine opens with compatibility conditions), constructs the closed subscheme associated to an ideal sheaf via gluing, establishes functorial operations (pullback and pushforward), and develops the theory of kernels of morphisms and scheme-theoretic images. This provides the foundation for working with closed subschemes, vanishing ideals, and the Galois connection between ideal sheaves and closed sets on schemes.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `IdealSheafData` structure (ideals on affine opens with localization compatibility), establishes complete lattice structure, constructs vanishing ideals and support as a Galois connection, defines morphism kernels and proves support equals closure of range for quasi-compact morphisms, and establishes the kernel adjunction |
| Functorial.lean | Defines pullback (`comap`) and pushforward (`map`) of ideal sheaves along morphisms, proves they form a Galois connection, establishes functoriality properties (composition laws), and provides `subschemeMap` for restricting morphisms between closed subschemes |
| Subscheme.lean | Constructs the closed subscheme associated to an ideal sheaf by gluing `Spec(Γ(X,U)/I(U))` for affine opens U, defines the inclusion morphism `subschemeι`, proves it is a preimmersion and quasi-compact, establishes `Γ(𝒪ₓ/I, U) ≅ 𝒪ₓ(U)/I(U)`, defines the scheme-theoretic image of a morphism, and establishes the adjunction between ideal sheaves and schemes over Y via kernels |

## Subdirectories

(No subdirectories)

## Search Tags

ideal-sheaf algebraic-geometry schemes closed-subscheme vanishing-ideal support galois-connection kernel pullback pushforward functorial subscheme gluing quotient preimmersion quasi-compact scheme-theoretic-image adjunction morphism-kernel ideal-sheaf-data affine-opens localization zariski-topology closed-sets
