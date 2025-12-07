---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Shapes/Pullback/Categorical
generated: 2025-12-07T15:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Categorical

## Overview

The `Categorical/` directory implements categorical pullbacks in the (2,1)-categorical sense, extending the ordinary pullback API to the 2-categorical setting where functors and natural transformations form the morphisms. A categorical pullback of functors F : A ⥤ B and G : C ⥤ B is a category of triples (a : A, c : C, F(a) ≅ G(c)), equipped with projection functors and a universal property for 2-commutative squares. The directory also establishes 2-functoriality via categorical cospan transformations, enabling systematic transformation of categorical pullbacks through functor diagrams with 2-commutative squares.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of CategoricalPullback F G as category of triples (a : A, c : C, F.obj a ≅ G.obj c) with projections π₁, π₂; establishes universal property via equivalence functorEquiv between X ⥤ (F ⊡ G) and CatCommSqOver F G X; includes 2-functoriality via CatCommSqOver.transform and CatCommSqOver.precompose for whiskering operations |
| CatCospanTransform.lean | Defines categorical cospan transformations (diagrams of functors A ⥤ A', B ⥤ B', C ⥤ C' with 2-commutative squares) and their morphisms; establishes bicategorical structure with composition, whiskering operations (◁, ▷), coherence isomorphisms (associator, unitors), and pentagon/triangle identities for 2-functoriality of categorical pullback construction |

## Subdirectories

(none)

## Search Tags

categorical-pullback 2-categorical functor-pullback natural-isomorphism cat-comm-sq universal-property functorEquiv CategoricalPullback projection-functor categorical-cospan cospan-transformation 2-commutative-square whiskering bicategory coherence-isomorphism associator unitor pentagon-identity triangle-identity Kerodon
