---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian/GrothendieckAxioms
generated: 2025-12-07T08:51:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# GrothendieckAxioms

## Overview

The `GrothendieckAxioms/` directory provides a formalization of Grothendieck's AB axioms for abelian categories, specifically focusing on exactness properties of limits and colimits. The core axioms AB4 and AB5 characterize when coproducts and filtered colimits preserve finite limits (left exactness). The directory includes basic definitions, theorems about pulling back connected colimits, and instances showing that various categories (types, functor categories, sheaf categories, ind-categories) satisfy these axioms.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `HasExactColimitsOfShape` and `HasExactLimitsOfShape`; defines AB4 (exact coproducts) and AB5 (exact filtered colimits); proves AB5 implies AB4; establishes invariance under equivalences |
| Colim.lean | Exactness properties of colimits; translates preservation of monomorphisms/epimorphisms from colimit functors to arbitrary cocones; proves inclusion morphisms into filtered colimits are monomorphisms under AB5 |
| Connected.lean | Pulling back connected colimits along morphisms; shows that pullbacks of colimit cocones are again colimit cocones when the indexing category is connected and colimits are exact; provides `hom_ext` principles for morphisms factoring through colimits |
| FunctorCategory.lean | Shows functor categories `C ⥤ A` inherit exact colimits/limits from `A`; instances for `HasExactColimitsOfShape` and `HasExactLimitsOfShape` in functor categories |
| Indization.lean | Shows the category of ind-objects `Ind C` satisfies AB5 when `C` has finite limits; proves `Ind C` is Grothendieck abelian when `C` is small and abelian |
| Sheaf.lean | AB axioms for sheaf categories; proves sheaf categories `Sheaf J A` are Grothendieck abelian when `A` is Grothendieck abelian and the topology is on a small category; handles filtered colimits and exactness in sheaf categories |
| Types.lean | Instance showing the category of types satisfies AB5 (filtered colimits commute with finite limits in `Type v`) |

## Subdirectories

(none)

## Search Tags

grothendieck-axioms ab4 ab5 exact-colimits exact-limits filtered-colimits abelian-categories functor-categories sheaf-categories ind-objects connected-colimits pullback-colimits left-exactness preservation-of-limits
