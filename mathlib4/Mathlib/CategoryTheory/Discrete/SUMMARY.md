---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Discrete
generated: 2025-12-07T08:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Discrete

## Overview

The `Discrete/` directory formalizes discrete categories—categories where the only morphisms are identities. It provides the `Discrete α` wrapper that promotes any type `α` to a category with only identity morphisms (technically encoded as `ULift (PLift (X = Y))` to satisfy universe constraints), along with functors, natural transformations, and equivalences between discrete categories and type-level operations. The directory also proves that discrete categories are closed under products and sums, and provides equivalences between structured arrow categories and the base category when the target is discrete with a unique element.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core discrete category construction: `Discrete α` structure, category instance with morphisms as wrapped equalities, `Discrete.functor` promoting functions to functors, `Discrete.natTrans` and `Discrete.natIso` for natural transformations/isomorphisms, equivalences between types and discrete categories, opposite category equivalence, `IsDiscrete` typeclass for categories with at most one morphism between objects |
| StructuredArrow.lean | Equivalences `StructuredArrow (Discrete.mk t) F ≌ C` and `CostructuredArrow F (Discrete.mk t) ≌ C` when the functor `F : C ⥤ Discrete T` targets a discrete category on a type with unique element |
| SumsProducts.lean | Product and sum constructions for discrete categories: `Discrete.productEquiv` showing `Discrete (J × K) ≌ Discrete J × Discrete K`, `Discrete.sumEquiv` showing `Discrete (J ⊕ K) ≌ Discrete J ⊕ Discrete K`, `IsDiscrete` instances for products and sums of discrete categories |

## Subdirectories

(none)

## Search Tags

discrete-categories identity-morphisms discrete-functor type-equivalence categorical-equivalence products-sums structured-arrows isDiscrete small-categories universe-lifting
