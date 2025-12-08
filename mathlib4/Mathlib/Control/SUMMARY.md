---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Control
generated: 2025-12-08T18:00:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 13
subdirs_count: 5
---

# Control

## Overview

The `Control/` directory provides comprehensive abstractions for functional programming patterns in Lean 4, organized around the core concepts of functors, applicatives, monads, and their transformers. It contains 13 base files covering fundamental constructs (functor composition, bifunctors, constant functors), monad transformers with lawfulness proofs (StateT, ReaderT, ExceptT), traversable and bitraversable structures with complete instance hierarchy, specialized monads (continuation, writer), fixed-point operators, random generation infrastructure, and universe-lifting utilities. Five subdirectories extend this foundation with multivariate functor theory, equivalence-preserving functors, traversability for both single-parameter and bifunctors, and advanced monad utilities including normalization infrastructure and continuation-passing style support.

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

- [x] `Bitraversable/` - Bitraversable typeclass for bifunctors supporting simultaneous traversal over both type parameters; includes lawful instances for Prod/Sum/Const/flip/bicompl/bicompr, partial traversal utilities (tfst/tsnd), and proof automation; enables applicative effects when mapping over data structures with two independently variable type parameters
- [x] `EquivFunctor/` - EquivFunctor typeclass instances for endofunctors of Type's "core" that map equivalences to equivalences coherently; provides implementations for Unique/Perm/Finset/Fintype with functor law proofs, enabling the equiv_rw tactic to rewrite under these type constructors
- [x] `Functor/` - Multivariate functor theory (MvFunctor) generalizing functors from types to type vectors (TypeVec n → Type); includes lawful instances, predicate/relation lifting (LiftP/LiftR) for type vectors, support sets for extracting values, and equivalence-based functor construction
- [x] `Monad/` - Advanced monad constructs: continuation monad (ContT/Cont) with callCC for control flow, writer monad (WriterT/Writer) for accumulating appendable state, monadic normalization infrastructure (functor_norm/monad_norm attributes), and extensionality tools for transformer equality; includes monad transformer composition instances
- [x] `Traversable/` - Complete traversable functor theory: core typeclass with traverse function, lawful instances (Option/List/Sum/Id) with identity/composition/naturality proofs, applicative transformations between functors, derived lemmas (map_traverse/traverse_map commutation), and equivalence transfer mechanism enabling reuse of instances via type isomorphisms

## Search Tags

control-theory functors applicatives monads monad-transformers bifunctors bitraversable traversable foldable lawful-instances functor-composition random-generation fixed-points state-monad reader-monad except-monad continuation-monad writer-monad universe-lifting type-classes functional-programming multivariate-functors equiv-functor predicate-lifting relation-lifting callcc continuation-passing-style natural-transformations applicative-transformations monadic-normalization functor-laws lawful-traversable lawful-bifunctor TypeVec MvFunctor compose-functors const-functor bifunctor-composition
