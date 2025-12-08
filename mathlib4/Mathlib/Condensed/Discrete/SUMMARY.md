---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Condensed/Discrete
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 5
subdirs_count: 0
---

# Discrete

## Overview

The `Discrete/` directory implements the theory of discrete condensed objects, providing functorial relationships between ordinary categories and their condensed counterparts. It establishes that discrete condensed objects (constant sheaves) are left adjoint to the forgetful functor that evaluates at a point, and characterizes discrete condensed objects through multiple equivalent conditions including locally constant representations and colimit-preserving properties. The directory provides these adjunctions and characterizations for both condensed sets, condensed modules, light condensed sets, and light condensed modules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Discrete-underlying adjunction: defines `discrete` functor (constant sheaf) and `underlying` functor (evaluation at point); proves `discrete ⊣ underlying` for both `Condensed C` and `LightCondensed C` |
| Characterization.lean | Characterizes discrete condensed objects via TFAE proofs: proves 5-7 equivalent conditions for discreteness including isomorphisms with constant sheaves, locally constant functors, and colimit preservation; applies to condensed sets/modules and light variants |
| Colimit.lean | Left Kan extension from finite sets to profinite sets: proves locally constant presheaves take cofiltered limits to colimits; establishes that condensed sets preserving these colimits are isomorphic to locally constant functors |
| LocallyConstant.lean | Locally constant functor and adjunction: defines functor `LocallyConstant - X` from sets to condensed sets; proves it's left adjoint to underlying functor via counit using fiber decomposition; establishes natural isomorphism with constant sheaf functor |
| Module.lean | Discrete condensed modules: extends locally constant functor to modules; proves `LocallyConstant.functor` for modules is naturally isomorphic to `discrete`; establishes adjunction with underlying module functor for both condensed and light condensed modules |

## Subdirectories

*(No subdirectories)*

## Search Tags

discrete-condensed constant-sheaf adjunction locally-constant fiber-decomposition left-kan-extension cofiltered-limits colimit-preservation characterization-theorem tfae condensed-modules light-condensed forgetful-functor evaluation-at-point profinite-limits finite-products presheaf-theory
