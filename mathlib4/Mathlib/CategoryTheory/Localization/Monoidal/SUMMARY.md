---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Localization/Monoidal
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Monoidal

## Overview

The `Monoidal/` directory develops the theory of localization for monoidal categories, constructing monoidal structures on localized categories when the morphism property being inverted is compatible with the monoidal structure. Given a monoidal category `C` and a morphism property `W` satisfying `W.IsMonoidal` (multiplicative and stable under whiskering), a localization functor `L : C ⥤ D` induces a monoidal structure on the localized category `D` such that `L` is a monoidal functor. The construction extends to braided and symmetric monoidal categories, and includes universal property results showing that functors lifting along monoidal localizations are themselves monoidal.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core construction of monoidal structure on localized categories via `LocalizedMonoidal L W ε` type synonym, defines `W.IsMonoidal` predicate (multiplicative + stable under left/right whiskering), constructs localized tensor product as bifunctor via `lift₂`, defines associator, left/right unitors, and proves pentagon/triangle coherence axioms using essential surjectivity to reduce to source category |
| Braided.lean | Localization of braided and symmetric monoidal categories, constructs braiding on `LocalizedMonoidal L W ε` as natural isomorphism between `tensorBifunctor` and its flip using `lift₂NatIso`, proves hexagon identities for braided structure, shows localization functor is braided monoidal, extends to symmetric case |
| Functor.lean | Universal property for monoidal structure on functors out of localized categories: given monoidal localization `L : C ⥤ D` and functor `F : D ⥤ E` lifting to monoidal functor `G : C ⥤ E`, constructs canonical monoidal structure on `F` via `functorMonoidalOfComp`, proves lifting isomorphism is monoidal natural transformation, uses `lift₂NatIso` to build `curriedTensorPreIsoPost` isomorphism |

## Subdirectories

*(none)*

## Search Tags

monoidal-category localization monoidal-functor whiskering multiplicative bifunctor tensor-product associator unitor pentagon triangle braided-category symmetric-monoidal braiding hexagon universal-property lifting monoidal-natural-transformation coherence
