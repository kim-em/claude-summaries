---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/Sheaf
generated: 2026-01-24T21:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Sheaf

## Overview

The `Sheaf/` directory provides sheaf-theoretic constructions for smooth manifolds in Mathlib. It defines sheaves of smooth functions from a manifold `M` to a target manifold `N`, upgrading these to sheaves of groups, rings, or commutative rings when the target carries additional algebraic structure. The key result is that smooth manifolds can be viewed as locally ringed spaces, with the structure sheaf being the sheaf of smooth scalar-valued functions. The stalks of this structure sheaf are local rings, with units being exactly the germs of functions nonzero at the stalk point.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Generic construction of sheaves from `LocalInvariantProp` on manifolds; defines `localPredicate` lifting local invariant properties to sheaf predicates and the general sheaf construction |
| Smooth.lean | Sheaf of smooth functions `smoothSheaf`; upgrades to `smoothSheafGroup`, `smoothSheafCommGroup`, `smoothSheafRing`, `smoothSheafCommRing` when target has algebraic structure; evaluation maps from stalks; surjectivity of stalk evaluation |
| LocallyRingedSpace.lean | Equips smooth manifolds with locally ringed space structure via `IsManifold.locallyRingedSpace`; proves stalks are local rings by characterizing units as germs nonzero at the point |

## Subdirectories

*(none)*

## Search Tags

sheaf smooth-sheaf structure-sheaf locally-ringed-space local-ring stalk germ evaluation smooth-functions presheaf local-invariant-prop lift-prop lie-group commutative-ring manifold-algebra
