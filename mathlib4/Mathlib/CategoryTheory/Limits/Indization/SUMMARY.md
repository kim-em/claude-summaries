---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Indization
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# Indization

## Overview

The `Indization/` directory provides the complete theory of ind-objects in category theory, implementing both the foundational definitions of ind-objects as filtered colimits of representable presheaves and the construction of the ind-completion `Ind C` as a category. It establishes ind-objects as presheaves that can be written as small filtered colimits of representables, proves recognition theorems characterizing them via properties of costructured arrow categories, and shows closure properties under filtered colimits and finite limits. The directory also constructs the ind-completion category with its canonical functors and proves fundamental theorems about limit and colimit existence in `Ind C`, making it the essential reference for working with ind-objects throughout mathlib's categorical infrastructure.

## Key Files

| File | Purpose |
|------|---------|
| IndObject.lean | Core definitions: `IndObjectPresentation` structure, `IsIndObject` predicate, recognition theorem relating ind-objects to filtered/finally-small costructured arrow categories, and left-exactness characterization for small finitely cocomplete categories |
| Category.lean | Construction of the ind-completion category `Ind C` as a locally small category, canonical functors `Ind.yoneda : C ⥤ Ind C` and `Ind.inclusion : Ind C ⥤ Cᵒᵖ ⥤ Type v`, and theorems on limit/colimit existence (6.1.17, 6.1.18, 6.1.8, 6.1.6 from Kashiwara-Schapira) |
| FilteredColimits.lean | Proof that ind-objects are closed under filtered colimits (Theorem 6.1.8), using interchange of filtered colimits with finite limits and pullout of colimits from hom functors |
| Equalizers.lean | Proof that ind-objects are closed under equalizers when `C` has equalizers (Proposition 6.1.17(i)), via presentations of parallel pairs as diagrams in functor categories |
| ParallelPair.lean | `IndParallelPairPresentation` structure showing parallel natural transformations between ind-objects can be commonly presented by diagrams and transformations in filtered functor categories (Proposition 6.1.15) |
| Products.lean | Proof that ind-objects are closed under products when `C` has products (Proposition 6.1.16(ii)), using commutativity of filtered colimits with products |
| LocallySmall.lean | Proof that the full subcategory of ind-objects is locally small (hom-sets live in universe `v`), via equivalence between natural transformations `colimit (F ⋙ yoneda) ⟶ G` and limits `limit (F.op ⋙ G)` |

## Subdirectories

(none)

## Search Tags

ind-objects ind-completion indization filtered-colimits representable-presheaves costructured-arrow finally-small left-exact-functors parallel-pairs equalizers products locally-small kashiwara-schapira colimit-presentations recognition-theorem ind-category yoneda-embedding presheaf-categories universal-properties closure-properties
