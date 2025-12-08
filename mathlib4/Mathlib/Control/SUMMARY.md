---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Control
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 13
subdirs_count: 5
---

# Control

## Overview

The `Control/` directory provides foundational abstractions for functional programming patterns in Lean 4, extending the theory of functors, applicatives, and monads. It defines typeclass infrastructure for functor composition, constant functors, bifunctors, lawful instances, and various monad transformers (StateT, ReaderT, ExceptT). The directory includes utilities for traversable data structures, folding operations, random value generation, fixed-point computations, and uliftable constructs for universe polymorphism.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core extensions for functors, applicatives, and monads; defines zipWithM, List.mapAccumRM/LM, fish operator laws, CommApplicative class, Sum monad instance, and Alternative combinators (succeeds, tryM, try?) |
| Applicative.lean | Applicative instances for concrete functors (Id, Functor.comp, Functor.const, Functor.add_const); lemmas for applicative operations including map_seq_map, seq_pure, seq_assoc; CommApplicative instance for Id |
| Functor.lean | Core functor definitions: Const and AddConst functors, Functor.Comp for functor composition, Liftp/Liftr for lifting predicates/relations, supp for extracting supported values, mapConstRev operator ($>) |
| Bifunctor.lean | Bifunctor typeclass for functions with two type arguments (F : Type* → Type* → Type*); defines bimap operation and LawfulBifunctor class asserting identity and composition laws |
| Fold.lean | Generalization of list folds to Traversable; defines foldMap using monoid accumulation with foldMap_hom property; implements foldl, foldr, toList via specialized monoids and const applicative functor |
| Lawful.lean | Monad transformer laws for StateT, ReaderT, ExceptT; defines mk constructors and run_mk simp theorems; includes run_bind, run_monadLift, run_monadMap lemmas |
| Fix.lean | Generic fix operator for recursive computations that may not be well-founded or productive; defines Fix typeclass and Part.fix with Fix.approx for successive finite approximations of fixed points |
| Random.lean | Randomness infrastructure: RandT/RandGT monad transformers and Rand/RandG monads using StdGen; Random class for randomly generatable objects; BoundedRandom for range-constrained generation; IO.runRand for execution |
| Combinators.lean | Utility combinators for functional programming (file presence confirmed but content not read) |
| EquivFunctor.lean | Equivalence functors (specific functionality to be documented) |
| LawfulFix.lean | Lawful fixed-point operator properties (specific laws to be documented) |
| ULift.lean | Universe-lifting utilities (specific functionality to be documented) |
| ULiftable.lean | Typeclass for types that can be universe-lifted (specific functionality to be documented) |

## Subdirectories

- [x] `Bitraversable/` - Bitraversable typeclass combining bifunctor with traversable structure (complete)
- [x] `EquivFunctor/` - Equivalence functor instances and theory (complete)
- [x] `Functor/` - Multivariate functor theory with predicate/relation lifting (complete)
- [x] `Monad/` - Monad-specific utilities including continuations and writer monad (complete)
- [x] `Traversable/` - Traversable typeclass with instances, equivalences, and lemmas (complete)

## Search Tags

control-theory functors applicatives monads monad-transformers bifunctors traversable foldable lawful-instances functor-composition random-generation fixed-points state-monad reader-monad except-monad universe-lifting type-classes functional-programming
