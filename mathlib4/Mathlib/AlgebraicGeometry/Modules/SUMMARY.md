---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/Modules
generated: 2025-12-04T04:51:34Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Modules

## Overview

The `Modules/` directory provides the theory of sheaves of modules over schemes in algebraic geometry. It defines the category of presheaves and sheaves of modules over a scheme X (denoted X.Modules), establishes this category as abelian, and constructs the fundamental tilde construction M^~ that associates to any R-module M a sheaf of modules over Spec R. The tilde construction includes the proof that stalks of M^~ are isomorphic to localizations of M, providing the essential connection between algebraic modules and geometric sheaves.

## Key Files

| File | Purpose |
|------|---------|
| Presheaf.lean | Defines the category X.PresheafOfModules of presheaves of modules over a scheme X, introduces X.ringCatSheaf as the underlying sheaf of rings (forgetting commutativity) |
| Sheaf.lean | Defines X.Modules as the abelian category of sheaves of modules over a scheme X, establishes sheafification and abelian category structure |
| Tilde.lean | Constructs the tilde functor M ↦ M^~ from R-modules to sheaves of 𝒪_{Spec R}-modules, proves stalk isomorphism (M^~)_x ≅ M_x (localization at prime ideal x), defines locally-fraction predicate and structure |

## Subdirectories

_(none)_

## Search Tags

algebraic-geometry sheaves modules quasi-coherent presheaf tilde-construction localized-module structure-sheaf spec-functor stalk-isomorphism abelian-category sheafification locally-fraction module-category scheme-modules
