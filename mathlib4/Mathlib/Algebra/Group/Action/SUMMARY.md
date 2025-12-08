---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Action
generated: 2025-12-01T23:58:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 16
subdirs_count: 1
---

# Action

## Overview

The `Action/` directory defines the foundational theory of group actions in mathlib4, providing the core typeclasses (`MulAction`, `AddAction`, `DistribMulAction`) that formalize how monoids and groups act on types, along with supporting concepts for analyzing action properties. It includes the fundamental definitions that extend the basic scalar multiplication notation (`SMul`/`VAdd`) with the monoid/group axioms, interaction typeclasses for composing multiple actions (`SMulCommClass`, `IsScalarTower`), and a comprehensive library of properties and constructions including faithful actions, pretransitive actions, action homomorphisms, endomorphism/automorphism representations, and equidecompositions. The `Pointwise/` subdirectory extends these individual-element actions to collective operations on sets and finsets, providing the infrastructure for pointwise algebraic operations throughout mathlib. This directory forms the theoretical foundation for all higher-level action theory in mathlib, including the module hierarchy.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass definitions for group actions; defines `MulAction M α` (monoid action with axioms `1 • b = b` and `(x * y) • b = x • y • b`), `AddAction G P` (additive analogue), `DistribMulAction M A` (action distributing over addition), and interaction typeclasses `SMulCommClass`, `IsScalarTower`, `IsCentralScalar` for composing multiple actions |
| Basic.lean | Comprehensive lemma library for group actions requiring more imports than Defs; includes `MulAction.toPerm` converting group actions to permutations, bijectivity/injectivity/surjectivity lemmas for actions, cancellation properties, and invertible element theory for actions |
| End.lean | Connections between actions and endomorphisms/automorphisms; provides tautological actions by `Function.End α` and `Equiv.Perm α` on types, and establishes equivalence between monoid/group actions and homomorphisms to endomorphism/automorphism structures via `MulAction.toEndHom` and `MulAction.toPermHom` |
| Faithful.lean | Faithful action typeclasses `FaithfulSMul M α` and `FaithfulVAdd G P`; actions where distinct group elements act differently (i.e., `(∀ a, m₁ • a = m₂ • a) → m₁ = m₂`); includes injectivity lemmas and instances for cancellative monoids |
| Pretransitive.lean | Pretransitive action typeclass `MulAction.IsPretransitive M α` where for any two points there exists a group element mapping one to the other (`∀ x y, ∃ g, g • x = y`); provides `exists_smul_eq` and `surjective_smul` interface; transitive actions are pretransitive + nonempty |
| Equidecomp.lean | Equidecomposition theory for group actions; defines equidecompositions of sets via bijections where each point is moved by an element from a finite set of group elements; implements equidecompositions as `PartialEquiv X X` with finiteness constraint; foundation for Banach-Tarski paradox formalization |
| Hom.lean | Action homomorphisms and equivariant maps (functions commuting with group actions) |
| Opposite.lean | Actions by opposite groups (reversing multiplication order) |
| Option.lean | Action instances on the `Option` type |
| Pi.lean | Action structures on dependent function types (pi types) |
| Prod.lean | Action structures on product types `α × β` |
| Sigma.lean | Action structures on sigma types (dependent sums) |
| Sum.lean | Action structures on sum types (disjoint unions) |
| TypeTags.lean | Alternative action structures using type tags |
| Units.lean | Actions by units (invertible elements) in monoids; provides `Units.mulAction` and related theory |
| TransferInstance.lean | Transferring action instances across type equivalences |

## Subdirectories

- [x] `Pointwise/` - Pointwise actions on sets and finsets

## Search Tags

group-action monoid-action mul-action add-action scalar-multiplication smul vadd faithful-action pretransitive-action transitive-action equidecomposition equivariant action-homomorphism endomorphism automorphism permutation distributive-action scalar-tower smul-comm-class typeclass pi-action product-action opposite-action units to-additive
