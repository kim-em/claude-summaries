---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/FreeMonoid
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# FreeMonoid

## Overview

The `FreeMonoid/` directory provides the free monoid construction over an arbitrary type, implemented as a synonym for `List α` with multiplication given by list concatenation. This directory includes the foundational definition with universal property (`FreeMonoid α ≃ (α → M) for any monoid M`), supporting operations (length, membership, map, reverse), homomorphism counting functions, finite set of unique symbols, and the proof that free monoids satisfy the `TwoUniqueProds` property for factorization uniqueness.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core free monoid definition as `List α` with monoid structure via concatenation, universal property (`lift : (α → M) ≃ (FreeMonoid α →* M)`), embedding `of : α → FreeMonoid α`, operations (length, membership, map, reverse), induction principles, and multiplicative action construction |
| Count.lean | Bundled homomorphisms for counting: `countP : FreeMonoid α →* Multiplicative ℕ` counts elements satisfying a predicate, `count : FreeMonoid α →* Multiplicative ℕ` counts occurrences of a specific element, wrapping `List.countP` and `List.count` |
| Symbols.lean | `symbols : FreeMonoid α → Finset α` extracts the finite set of unique symbols appearing in a free monoid element via `List.toFinset`, with lemmas for `symbols_one = ∅`, `symbols_mul = union`, membership characterization |
| UniqueProds.lean | Instance proving `FreeMonoid κ` has the `TwoUniqueProds` property (unique factorization into products of two elements) by using length as a homomorphism to `Multiplicative ℕ` and applying `List.append_inj` |

## Subdirectories

*(none)*

## Search Tags

free-monoid list concatenation universal-property monoid-homomorphism lift embedding count symbols unique-products factorization additive-free-monoid
