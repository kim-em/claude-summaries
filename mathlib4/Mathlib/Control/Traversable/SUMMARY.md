---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Control/Traversable
generated: 2025-12-08T17:30:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# Traversable

## Overview

The `Traversable/` directory provides the complete theory of traversable functors in Lean 4, including the core typeclass definition, lawful instances, properties, and methods for transferring traversability across type equivalences. Traversable functors generalize functors by allowing effectful functions to be mapped over collections while maintaining the collection structure, enabling patterns like `traverse f : List α → IO (List β)` from functions `f : α → IO β`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `Traversable` typeclass with `traverse` function, `LawfulTraversable` with identity/composition/naturality laws, `ApplicativeTransformation` typeclass for natural transformations between applicative functors, `sequence` function for effectful collection composition, instances for Id/Option/List/Sum |
| Instances.lean | Lawful traversable instances for standard types (Option, List, Sum σ); proves all required laws (id_traverse, comp_traverse, traverse_eq_map_id, naturality) for each instance with detailed case analysis and functor_norm simplification |
| Lemmas.lean | Derived properties and equivalences: `PureTransformation` natural transformation from Id to F, proofs that `map = traverse ∘ pure`, `map_traverse` and `traverse_map` commutation lemmas, `pure_traverse`, `id_sequence`, `comp_sequence`, naturality for sequence |
| Equiv.lean | Transfer mechanism for traversable structure across type equivalences: `Equiv.map`/`Equiv.functor` for functoriality, `Equiv.traverse`/`Equiv.traversable` for traversability, proofs that lawfulness is preserved under equivalence (`Equiv.isLawfulTraversable`), enabling reuse of instances via isomorphisms |

## Subdirectories

*(none)*

## Search Tags

traversable functors applicative-functors lawful-traversable traverse sequence applicative-transformation natural-transformation functor-composition id-traverse comp-traverse naturality equivalence-transfer option-instance list-instance sum-instance effectful-operations functor-laws type-classes functional-programming
