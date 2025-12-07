---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Generator
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 8
subdirs_count: 0
---

# Generator

## Overview

The `Generator/` directory formalizes the theory of generators, separators, detectors, and their dual notions in category theory. It provides several non-equivalent characterizations of generating objects including separating sets (families of representable functors that are collectively faithful), detecting sets (families that collectively reflect isomorphisms), and strong generators (generators with additional factorization properties). The module covers applications to preadditive categories, abelian categories, presheaves, sheaves, homological complexes, and ind-objects, establishing existence results for separators in various categorical contexts.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `IsSeparating`, `IsCoseparating`, `IsDetecting`, `IsCodetecting` for object properties with singleton versions `IsSeparator`, `IsCoseparator`, `IsDetector`, `IsCodetector`, and proofs relating these notions under categorical assumptions (equalizers, balanced categories, etc.) |
| StrongGenerator.lean | Strong generators: object properties that are separating and detect non-surjective monomorphisms via factorization, with characterization via extremal epimorphisms from coproducts |
| Preadditive.lean | Characterizations of separators in preadditive categories: separator iff all morphisms annihilated by it are zero, with Yoneda-style characterizations via `preadditiveCoyoneda` and `preadditiveYoneda` |
| Abelian.lean | Freyd's theorem: complete abelian categories with enough injectives and a separator have an injective coseparator (and dual result for enough projectives) |
| Presheaf.lean | Construction of separators in presheaf categories `Cᵒᵖ ⥤ A`: if `A` has a separator and suitable coproducts, then `Cᵒᵖ ⥤ A` has a separator via free Yoneda construction |
| Sheaf.lean | Extension to sheaves: if `A` is preadditive with a separator and suitable coproducts, then `Sheaf J A` has a separator for any Grothendieck topology `J` |
| HomologicalComplex.lean | Separators in `HomologicalComplex C c`: if `C` has a separator, then `HomologicalComplex C c` has a separating family (and separator with coproducts) indexed by pairs of a separator and a degree |
| Indization.lean | The Yoneda embedding into ind-objects provides a separating set in `Ind C`, yielding a separator when `C` is small preadditive with finite colimits |

## Subdirectories

*(No subdirectories)*

## Search Tags

category-theory generators separators detectors representing-objects faithful-functors reflection-isomorphisms preadditive-categories abelian-categories presheaves sheaves homological-complexes ind-objects yoneda-lemma strong-generators extremal-epimorphisms grothendieck-topology well-powered-categories
