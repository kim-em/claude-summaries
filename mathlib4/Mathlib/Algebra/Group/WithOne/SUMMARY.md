---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/WithOne
generated: 2025-12-01T18:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# WithOne

## Overview

This folder implements the `WithOne` construction that adjoins a unit element to a semigroup to obtain a monoid, along with its additive dual `WithZero` that adjoins a zero element. The construction is defined as `Option α` and provides the free functor from semigroups to monoids. The folder includes core definitions, algebraic instances (showing `WithOne α` is a monoid when `α` is a semigroup), bundled homomorphisms for lifting and mapping operations, and utilities for working with the coproduct structure.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `WithOne α` as `Option α`, coercion from `α`, instances for `One`, `Mul`, `Inv`, `MulOneClass`, `Monoid`, `CommMonoid`; recursion principles `recOneCoe` and eliminators `unone`; basic lemmas about coercion injectivity and distinguishing `1` from coerced elements |
| Basic.lean | Bundled morphisms and lifting: `coeMulHom` for coercion as a semigroup homomorphism, `lift` equivalence between semigroup homomorphisms `α →ₙ* β` and monoid homomorphisms `WithOne α →* β`, `mapMulHom` for lifting multiplicative maps, and `MulEquiv.withOneCongr` for equivalences |
| Map.lean | Unbundled map operations: `WithOne.map` for lifting arbitrary functions `α → β` via `Option.map`, and `WithOne.map₂` for lifting binary functions to the product, with lemmas about interaction with `1` and coercions |

## Subdirectories

(none)

## Search Tags

with-one with-zero adjoin-unit free-monoid option semigroup monoid lift-homomorphism coproduct adjunction algebraic-construction to-additive
