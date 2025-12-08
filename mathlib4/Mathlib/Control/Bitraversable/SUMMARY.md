---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Control/Bitraversable
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Bitraversable

## Overview

The `Bitraversable/` directory defines the bitraversable typeclass for bifunctors that support traversal operations over both type parameters simultaneously. It provides the core typeclass definitions, lawfulness properties, concrete instances (Prod, Sum, Const, flip, bicompl, bicompr), and utility lemmas for partial traversals (tfst/tsnd). This extends the standard traversable pattern to bifunctors, enabling applicative effects when mapping over data structures with two independently variable type parameters.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core bitraversable definitions: `Bitraversable` typeclass with bitraverse function, `LawfulBitraversable` class with identity/composition/naturality/bimap-equivalence laws, and bisequence utility for commuting applicative functors |
| Instances.lean | Concrete bitraversable instances for Prod (×), Sum (⊕), Const, flip, bicompl (bifunctor composed with two traversables), and bicompr (traversable composed with bifunctor); proves lawfulness for all instances; provides default Traversable instance for partially-applied bitraversables |
| Lemmas.lean | Utility functions tfst (traverse first parameter) and tsnd (traverse second parameter); composition and identity lemmas for tfst/tsnd; equivalence with bifunctor fst/snd operations in Id monad; functor_norm attributes for proof automation |

## Subdirectories

None.

## Search Tags

bitraversable bifunctor traversable applicative functor lawful-typeclass prod sum const flip bicompl bicompr tfst tsnd bisequence type-classes functional-programming composition-laws naturality
