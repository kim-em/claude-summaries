---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Endofunctor
generated: 2025-12-07T08:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Endofunctor

## Overview

The `Endofunctor/` directory contains the theory of algebras and coalgebras for endofunctors in category theory. An algebra of an endofunctor `F : C ⥤ C` consists of an object `A` and a structure morphism `F(A) → A`, while a coalgebra consists of an object `V` and a structure morphism `V → F(V)`. This formalization includes the category structures for both algebras and coalgebras, forgetful functors, and proves key results including that initial algebras have isomorphic structure maps and that adjunctions `F ⊣ G` induce equivalences between algebras over `F` and coalgebras over `G`.

## Key Files

| File | Purpose |
|------|---------|
| Algebra.lean | Defines algebras and coalgebras of endofunctors with their morphisms, category instances, forgetful functors, functors induced by natural transformations, and proves that initial algebra structure maps are isomorphisms and that adjunctions induce equivalences between algebra and coalgebra categories |

## Subdirectories

(none)

## Search Tags

endofunctor algebra coalgebra structure-morphism forgetful-functor initial-algebra terminal-coalgebra lambek-lemma adjunction category-equivalence natural-transformation fixed-point
