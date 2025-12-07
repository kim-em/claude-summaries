---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Category/Cat
generated: 2025-12-07T08:29:50Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# Cat

## Overview

The `Cat/` subdirectory contains advanced properties and constructions for the category of categories (`Cat`). It establishes that `Cat` has all small limits and colimits, is Cartesian closed, admits various adjunctions (with `Type` via discrete categories and connected components), supports opposite category operations, and provides functorial embeddings into larger universes via `AsSmall`. These results demonstrate that `Cat` itself has rich categorical structure.

## Key Files

| File | Purpose |
|------|---------|
| Limit.lean | Proves `Cat` has all small limits; constructs limit category with objects as limits of object functors and morphisms as limits of hom diagrams; shows `Cat.objects` preserves limits |
| Colimit.lean | Proves `Cat` has all small colimits by embedding as reflective subcategory of simplicial sets; uses nerve adjunction and homotopy category functor |
| CartesianClosed.lean | Establishes Cartesian closed structure on `Cat` with exponentials given by functor categories; defines currying and flipping isomorphisms; adjunction via currying |
| Adjunction.lean | Two key adjunctions: `typeToCat ⊣ Cat.objects` (discrete categories ↔ types) and `connectedComponents ⊣ typeToCat` (connected components of categories) |
| Op.lean | Defines `opFunctor : Cat ⥤ Cat` assigning opposite categories; proves strict involution and establishes `opEquivalence : Cat ≌ Cat` |
| AsSmall.lean | Functor `asSmallFunctor : Cat.{v,u} ⥤ Cat.{max w v u, max w v u}` embedding categories into larger universes via `AsSmall` construction |
| Terminal.lean | Characterizes terminal categories as discrete categories with unique object; proves `Cat` has terminal object; provides isomorphisms to `Discrete PUnit` |

## Subdirectories

(none)

## Search Tags

cat-limits cat-colimits cartesian-closed exponential-objects functor-categories adjunctions discrete-categories connected-components opposite-categories universe-lifting terminal-categories nerve-adjunction simplicial-sets
