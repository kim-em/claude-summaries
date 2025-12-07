---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian/Injective
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Injective

## Overview

The `Injective/` directory contains the theory of injective objects in abelian categories, including characterizations, injective dimension theory, resolutions, and extensions. It establishes that objects are injective iff their preadditive Yoneda functor preserves finite colimits, develops a complete dimension theory with Ext vanishing characterizations, constructs injective resolutions functorially up to homotopy equivalence, and provides extension machinery for cochain complexes.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Characterizes injective objects in abelian categories: `J` is injective iff `preadditiveYonedaObj J` preserves finite colimits, with instances showing preservation of homology and colimits |
| Dimension.lean | Injective dimension theory: defines `HasInjectiveDimensionLT X n` (all Ext groups vanish for degree ≥ n), proves dimension behaves correctly under isomorphisms/retracts/short exact sequences, and defines `injectiveDimension : C → WithBot ℕ∞` |
| Extend.lean | Extends injective resolutions from ℕ-indexed to ℤ-indexed cochain complexes; constructs quasi-isomorphism `R.ι' : (CochainComplex.singleFunctor C 0).obj X ⟶ R.cochainComplex` for any injective resolution `R` |
| Resolution.lean | Constructs injective resolutions in abelian categories with enough injectives via iterated syzygies; proves descents of morphisms between resolutions are unique up to homotopy, establishes homotopy equivalence of resolutions, and defines functorial `injectiveResolutions : C ⥤ HomotopyCategory C` |

## Subdirectories

None.

## Search Tags

injective-objects injective-resolutions injective-dimension ext-groups yoneda-functor preadditive-categories abelian-categories homotopy-category cochain-complexes quasi-isomorphism enough-injectives derived-functors homological-algebra syzygies dimension-theory exact-sequences
