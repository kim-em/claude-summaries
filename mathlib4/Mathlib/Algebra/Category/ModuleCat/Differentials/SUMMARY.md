---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ModuleCat/Differentials
generated: 2025-12-02T00:00:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Differentials

## Overview

The `Differentials/` directory develops the theory of Kähler differentials in the categorical framework of modules over commutative rings. It defines derivations relative to morphisms of commutative rings, constructs the universal module of differentials (Kähler differentials), and extends these concepts to presheaves of modules and commutative rings. This provides the foundation for studying differential structures in algebraic geometry through category theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `ModuleCat.Derivation` type for derivations relative to ring morphisms `f : A ⟶ B` with values in B-modules; constructs `CommRingCat.KaehlerDifferential f` as the universal module of differentials with its universal derivation `D`; provides functoriality via `map` for commutative squares; establishes universal property through `desc` map |
| Presheaf.lean | Extends differential theory to presheaves: defines `PresheafOfModules.Derivation φ` for morphisms of presheaves of commutative rings; formalizes universal derivation property; constructs `DifferentialsConstruction.relativeDifferentials'` as presheaf of Kähler differentials with universal derivation; proves `HasDifferentials` instance showing existence of universal derivations for presheaf morphisms |

## Subdirectories

None.

## Search Tags

kaehler-differentials derivations commutative-rings modules category-theory universal-properties presheaves algebraic-geometry differential-structures ring-morphisms
