---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic/Small
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Small

## Overview

The `Small/` directory implements the `Small.{w}` typeclass and related infrastructure for expressing that a type is "small" - i.e., embeddable into a specified universe level `w`. A type `α : Type v` is `Small.{w}` if there exists an equivalence `α ≃ S` for some `S : Type w`. This provides a noncomputable model `Shrink α : Type w` with an equivalence `equivShrink α : α ≃ Shrink α`, enabling universe polymorphism and controlling universe levels in formal proofs. The directory includes core definitions, typeclass instances for common type constructors (sigma, pi, prod, sum, quot), propagation theorems (`small_of_injective`, `small_of_surjective`), and specialized instances for lists and sets.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `Small.{w}` typeclass definition, `Shrink` model and `equivShrink` equivalence; includes `Small.mk'` constructor, basic instances (`small_self`, `small_lift`, universe-indexed instances), type constructor instances (sigma, ulift, plift), `small_congr` lemma for equivalence-preserving smallness, and proof that `Type (max u v)` is not `Small.{u}` (Cantor-style diagonalization); imports only Equiv.Defs for minimal dependencies |
| Basic.lean | Additional `Small` instances and fundamental theorems: `small_of_injective` and `small_of_surjective` for propagating smallness through functions, `small_subsingleton` for subsingleton types, `small_of_injective_of_exists` for indirect surjections, type constructor instances (pi, prod, sum, set, quot, quotient); asserts no dependency on `Countable` to maintain import order |
| List.lean | `Small` instances for `List α` and `Vector α n` types; proves `smallVector` via equivalence with `Fin n → α`, and `smallList` via sigma type over all lengths; kept separate from Basic.lean to avoid pulling in Data.Vector.Basic dependencies into low-level category theory imports |
| Set.lean | Comprehensive `Small` instances for set operations: subset propagation (`small_subset`), powerset, product sets, pi sets, range/image, unions (binary, indexed, bounded), intersections (with nonemptiness requirements), differences, separators, and concrete instances for empty/singleton/pair sets; proves `small_univ_iff` characterizing when the universal set is small |

## Subdirectories

(none)

## Search Tags

small universe-polymorphism universe-levels type-equivalence shrink embedding injective surjective subsingleton sigma-types product-types sum-types quotient-types sets lists vectors cantor-diagonal type-theory mathlib lean4
