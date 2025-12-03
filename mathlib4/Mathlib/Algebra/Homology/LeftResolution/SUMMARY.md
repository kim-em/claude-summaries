---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology/LeftResolution
generated: 2025-12-02T08:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# LeftResolution

## Overview

The `LeftResolution/` directory provides machinery for constructing functorial left resolutions (particularly projective resolutions) in abelian categories. Given a fully faithful functor `ι : C ⥤ A` to an abelian category, it defines a `LeftResolution` structure containing a functor `F : A ⥤ C` with natural epimorphisms `π.app X : ι.obj (F.obj X) ⟶ X`, and uses this to iteratively build chain complex resolutions `chainComplexFunctor : A ⥤ ChainComplex C ℕ`. Extensions to idempotent completions ensure zero morphism preservation for deriving functors on complexes.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `LeftResolution ι` structure with functor `F : A ⥤ C` and epimorphism `π`, iterative construction of `chainComplex : ChainComplex C ℕ` via kernels, exactness proofs, and `chainComplexFunctor` for functorial resolutions |
| Reduced.lean | Extension to idempotent completions: `karoubi` lifts resolutions to Karoubi envelopes with zero morphism preservation, `reduced` produces `LeftResolution ι` in idempotent complete categories where `F` preserves zero morphisms |
| Transport.lean | Transport left resolutions along category equivalences: `transport` moves `LeftResolution ι` to `LeftResolution ι'` via equivalences `A' ≌ A` and `C' ≌ C`, `ofCompIso` constructs resolutions from composed isomorphisms |

## Subdirectories

None.

## Search Tags

left-resolution projective-resolution functorial-resolution abelian-category derived-functor chain-complex resolution-functor epimorphism idempotent-completion karoubi-envelope zero-morphism category-equivalence transport homological-algebra
