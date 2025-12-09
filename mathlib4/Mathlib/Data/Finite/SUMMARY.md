---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Finite
generated: 2025-12-09T06:15:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 8
subdirs_count: 0
---

# Finite

## Overview

The `Finite/` directory implements the `Finite` typeclass and related constructions for finite types in Lean. Unlike `Fintype` which is computational and provides actual algorithms to enumerate elements, `Finite` is a proposition (`Prop`-valued) that merely asserts a type is in bijection with some `Fin n`, enjoying proof irrelevance and avoiding decidability requirements. This module provides the core definition, cardinality functions via `Nat.card`, instances for standard type constructors (products, sums, sigma types, vectors), and the dual notion of infinite types. It also defines `Set.Finite` for finite sets and proves their closure properties.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `Finite` typeclass (types equivalent to `Fin n`), `Infinite` typeclass (not finite), `Set.Finite` and `Set.Infinite` for finite/infinite sets; instances for `Bool`, `Prop`, `PLift`, `ULift` |
| Card.lean | Cardinality functions for finite types via `Nat.card α` (junk value 0 for infinite types); equivalences to `Fin (Nat.card α)`, cardinality inequalities via injective/surjective functions, set cardinality bounds |
| Perm.lean | Properties of permutation groups `Equiv.Perm α` on finite types; proves `Nat.card (Equiv.Perm α) = (Nat.card α)!` |
| Prod.lean | `Finite` instances for product types `α × β`, `PProd α β`, and dependent products `∀ a, β a`; `Set.Finite.prod` for Cartesian products of finite sets, `Set.Finite.image2` for binary images, off-diagonal products; infinite product characterizations |
| Set.lean | Additional lemmas about `Finite` and `Set`s: `Finite` of preimage under injective functions, `Finite` from finite range of injective functions |
| Sigma.lean | `Finite` instances for sigma types `Σ a, β a` and `Σ' i, π i` (psigma); finiteness follows from finite index type and finite fibers |
| Sum.lean | `Finite` instances for sum types `α ⊕ β` and `α ⊕' β` (psum); projection lemmas showing components are finite if sum is finite |
| Vector.lean | `Finite` instances for `Vector α n` (lists of fixed length n) and `Sym α n` (symmetric powers); finiteness follows from finite element type |

## Subdirectories

## Search Tags

finite-types finiteness finite-sets proposition-valued cardinality nat-card infinite-types proof-irrelevance type-constructors products sums sigma-types vectors permutations set-finite
