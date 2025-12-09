---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Fintype
generated: 2025-12-09T15:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 28
subdirs_count: 0
---

# Fintype

## Overview

The `Fintype/` directory defines the core typeclass for types with finitely many elements, along with its fundamental theory and instances. A `Fintype α` provides a complete enumeration of all elements of `α` as a `Finset`, enabling decidable computation over finite types. This directory includes basic instances (for `Fin`, products, sums, options, subtypes, etc.), cardinality theory, equivalences with `Fin n`, pigeonhole principles, operations on permutations, order-theoretic constructions, and integration with big operators. It bridges between the computational world (via `Finset`) and mathematical reasoning about finite types.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Fintype α` typeclass (a `Finset` of all elements with completeness proof), `Finset.univ`, and subtype instances |
| Basic.lean | Elementary `Fintype` instances for `Fin n`, products, sums, options, pi types; basic operations and lemmas |
| Card.lean | Cardinality function `Fintype.card α` returning the number of elements; cardinality lemmas for various type constructors |
| EquivFin.lean | Equivalences between `Fintype α` and `Fin (Fintype.card α)`; both computable (`truncEquivFin`) and noncomputable (`equivFin`) versions; equivalence between fintypes of equal cardinality |
| BigOperators.lean | Integration with big operators: products and sums over `Fintype`; derives cardinality results using algebraic operations |
| Sets.lean | Conversion between `Set α` and `Finset α` for finite types via `Set.toFinset`; equivalence `Fintype.finsetEquivSet` |
| Pigeonhole.lean | Pigeonhole principles: finitely many pigeons in fewer holes (`exists_ne_map_eq_of_card_lt`), infinitely many pigeons in finitely many holes (`Finite.exists_ne_map_eq_of_infinite`, `Finite.exists_infinite_fiber`) |
| Perm.lean | `Fintype` instances for `Equiv` and `Perm`; enumeration of all permutations via `permsOfFinset`; factorial cardinalities |
| Quotient.lean | Quotients of families indexed by finite types; lifting and recursion principles for `Π i : ι, Quotient (S i)` when `ι` is finite |
| Order.lean | Order-theoretic instances: `OrderBot`, `OrderTop`, `BoundedOrder` on fintypes with lattice structure; promotion to complete lattices (noncomputable) |
| Lattice.lean | Lemmas relating fintypes to order and lattice structure; `sup`/`inf` over universes as suprema/infima; existence of maxima |
| Option.lean | `Fintype` instance for `Option α`; card formula `card (Option α) = card α + 1`; inverse construction `fintypeOfOption` |
| Prod.lean | `Fintype` instance for products `α × β`; `univ = univ ×ˢ univ`; set-finset conversions for products |
| Sum.lean | `Fintype` instance for sums `α ⊕ β`; disjoint union enumeration |
| Sigma.lean | `Fintype` instance for dependent pairs `Σ a : α, β a` |
| Pi.lean | `Fintype` instance for dependent function types `Π a : α, β a` when domain and all codomains are finite |
| Vector.lean | `Fintype` instance for vectors `Vector α n` (lists of length n) |
| List.lean | `Fintype` instance for lists over a finite type (via quotient by permutation equivalence - not directly) |
| Powerset.lean | `Fintype` instance for powersets `Set α` when `α` is finite; card formula `card (Set α) = 2^(card α)` |
| Fin.lean | Additional `Fintype` lemmas specific to `Fin n` |
| OfMap.lean | Constructing `Fintype` instances via functions and embeddings |
| CardEmbedding.lean | Relationship between cardinalities and embeddings; bounds on number of embeddings |
| Inv.lean | `Fintype` instances for types with inversion operations |
| Parity.lean | `Fintype` instances related to parity (even/odd elements) |
| Shrink.lean | Type shrinking lemmas for finite types |
| Sort.lean | `Fintype` instances for sorted structures |
| Units.lean | `Fintype` instance for unit groups `αˣ` in finite types with multiplication |
| WithTopBot.lean | `Fintype` instances for types extended with top/bottom elements |

## Subdirectories

(none)

## Search Tags

fintype finite-types enumeration cardinality finset universe pigeonhole-principle permutations equivalences quotients order-theory lattice big-operators products sums options dependent-types
