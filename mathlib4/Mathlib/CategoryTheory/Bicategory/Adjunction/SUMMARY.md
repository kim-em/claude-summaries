---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory/Adjunction
generated: 2025-12-07T20:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Adjunction

## Overview

The `Adjunction/` directory formalizes adjunctions and mates in bicategories. It provides the core definition of adjunction between 1-morphisms with unit and counit satisfying triangle identities, constructs the bicategory of adjunctions (`Adj B`) where 1-morphisms are adjunctions and 2-morphisms are mate maps, and establishes the fundamental mate correspondence between 2-cells involving adjoint pairs through the `mateEquiv` and `conjugateEquiv` bijections.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core adjunction definition (`l ⊣ r`) with unit, counit, and triangle identities; adjoint equivalences; left/right adjoint typeclasses with axiom of choice extraction |
| Mate.lean | Mate correspondence via `mateEquiv` bijection between squares of left adjoints and right adjoints; `conjugateEquiv` for transformations between adjunctions; vertical/horizontal composition of mate squares; preservation of isomorphisms |
| Adj.lean | Bicategory of adjunctions `Adj B` with 1-morphisms as adjunctions and 2-morphisms as mate pairs; associators, unitors, whiskering via conjugate transformations; pseudofunctor `forget₁` to underlying left adjoints |

## Subdirectories

*(none)*

## Search Tags

adjunction bicategory unit counit triangle-identity mate-correspondence mateEquiv conjugateEquiv left-adjoint right-adjoint adjoint-equivalence 2-morphism whiskering bicategory-of-adjunctions transformation-of-adjoints
