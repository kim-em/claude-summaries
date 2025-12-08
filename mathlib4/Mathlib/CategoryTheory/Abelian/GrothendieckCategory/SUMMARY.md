---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian/GrothendieckCategory
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 6
subdirs_count: 1
---

# GrothendieckCategory

## Overview

The `GrothendieckCategory/` directory provides a complete formalization of Grothendieck abelian categories and their fundamental theorems. A Grothendieck category is an abelian category that is locally small, has exact filtered colimits (AB5), and has a separator. The directory establishes the core definition and proves invariance under categorical equivalences, demonstrates that Grothendieck categories have all limits and colimits and are well-powered, proves that monomorphisms are stable under transfinite composition, studies presentability properties via cardinal-filtered colimits of the coyoneda functor, and proves Grothendieck's fundamental theorem that every Grothendieck abelian category has enough injectives using the small object argument. The crowning achievement is the `ModuleEmbedding/` subdirectory, which proves the Gabriel-Popescu theorem showing that every Grothendieck abelian category embeds fully faithfully into a module category, along with dual embedding results for opposite categories. Together, these results demonstrate that Grothendieck categories, despite their abstract categorical definition, can be faithfully represented as concrete categories of modules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `IsGrothendieckAbelian` as locally small abelian category with AB5 and separator; proves invariance under equivalences, derives AB4, and shows Grothendieck categories have all limits and colimits and are well-powered |
| ColimCoyoneda.lean | Presentability properties: proves coyoneda functors preserve colimits of monomorphism diagrams indexed by κ-filtered categories for big enough regular cardinals κ; establishes injectivity and surjectivity lemmas via transfinite iteration |
| Coseparator.lean | Proves Grothendieck categories have a coseparator by constructing an injective coseparator from the separator using enough injectives |
| EnoughInjectives.lean | Grothendieck's theorem that every Grothendieck abelian category has enough injectives; uses small object argument applied to `generatingMonomorphisms G` (subobject inclusions of generator G); proves any monomorphism is a transfinite composition of pushouts of generating monomorphisms |
| Monomorphisms.lean | Proves monomorphisms in Grothendieck abelian categories are stable under transfinite composition (instance of `IsStableUnderTransfiniteComposition`) |
| Subobject.lean | Subobject lattice theory: relates colimits of functors `J ⥤ MonoOver X` from filtered categories to suprema in the complete lattice `Subobject X`; shows colimit monomorphism equals supremum of component subobjects |

## Subdirectories

- [x] `ModuleEmbedding/` - Module embedding theorems (Gabriel-Popescu)

## Search Tags

grothendieck-categories abelian-categories ab5 separator locally-small enough-injectives small-object-argument presentability cardinal-filtered transfinite-composition monomorphisms-stable subobject-lattice coyoneda-colimits injective-objects coseparator gabriel-popescu
