---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Dialectica
generated: 2025-12-07T09:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Dialectica

## Overview

The Dialectica category is an important categorical model of linear type theory, introduced by Valeria de Paiva in 1989. This folder contains the formalization of the Dialectica construction, which defines objects as triples `⟨U, X, α ⊆ U × X⟩` where `α` is a relation encoded as a subobject. Morphisms are pairs `(f : U ⟶ V, F : U ⨯ Y ⟶ X)` satisfying a relational condition expressed via pullbacks. Dialectica categories are significant models for linear logic that satisfy properties like independence of constants, with applications to quantum systems, programming effects, linear dependent types, polynomial functors, Petri nets, and state in imperative programming.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the Dialectica category structure `Dial C` with objects as source-target-relation triples, morphisms as pairs `(f, F)` with relational constraints, composition and identity, and isomorphism construction via source/target isomorphisms |
| Monoidal.lean | Proves that `Dial C` has a symmetric monoidal structure with tensor product combining components pairwise and relation as an infimum, including unitors, associator, and braiding isomorphisms |

## Subdirectories

*(No subdirectories)*

## Search Tags

dialectica-categories linear-type-theory linear-logic categorical-models subobjects relations polynomial-functors monoidal-categories symmetric-monoidal-categories de-paiva finite-products pullbacks
