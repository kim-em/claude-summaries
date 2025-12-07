---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Localization/CalculusOfFractions
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# CalculusOfFractions

## Overview

This directory contains specialized constructions and results for the calculus of fractions in localized categories. It extends the basic calculus of fractions framework with bundled structures for working with multiple fractions sharing common denominators (essential for preadditive categories), essential surjectivity results for functors on composable arrows, and specialized calculus deduced from adjunctions. These tools are crucial for computing morphisms in localized categories and establishing that localization preserves algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Fractions.lean | Defines bundled structures `LeftFraction₂` and `LeftFraction₃` for tuples of left fractions with shared denominators, equivalence relations on these tuples, and generalizations of fraction existence lemmas (`exists_leftFraction₂`, `exists_leftFraction₃`) needed for preadditive structure construction |
| Preadditive.lean | Constructs preadditive category structure on localized categories when source category is preadditive and morphism property has left calculus of fractions, proving localization functor is additive using shared-denominator fraction arithmetic |
| ComposableArrows.lean | Proves essential surjectivity of functor `L.mapComposableArrows n : ComposableArrows C n ⥤ ComposableArrows D n` when `L` is localization functor for morphism property with left or right calculus of fractions, important for coherence results |
| OfAdjunction.lean | Shows that for adjunction `G ⊣ F` with `F` fully faithful, if `W` is inverted by `G` and unit/counit morphisms belong to `W`, then `G` is localization functor and `W` has calculus of fractions, specialized to case where `W` is inverse image of isomorphisms |

## Subdirectories

None.

## Search Tags

calculus-of-fractions localization category-theory shared-denominator left-fraction right-fraction preadditive-localization additive-functor composable-arrows essential-surjectivity adjunction fully-faithful gabriel-zisman
