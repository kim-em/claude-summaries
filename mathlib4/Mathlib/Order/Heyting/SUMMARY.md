---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Heyting
generated: 2026-01-26T01:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Heyting

## Overview

The `Heyting/` directory provides the core formalization of Heyting algebras and their dual structures (co-Heyting algebras and bi-Heyting algebras) in Lean's Mathlib. Heyting algebras are bounded distributive lattices with an implication operation `⇨` satisfying an adjunction property, serving as the order-theoretic model of intuitionistic logic. The directory includes basic definitions and theorems, homomorphisms preserving Heyting structure, the co-Heyting boundary operator (corresponding to topological boundary), and a proof that regular elements (those satisfying `aᶜᶜ = a`) form a Boolean algebra, enabling classical reasoning within intuitionistic logic.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of (generalized) Heyting, co-Heyting, and bi-Heyting algebras with their fundamental operations (`⇨`, `\`, `ᶜ`, `￢`) and extensive API for implication/difference/complement operations, distributivity laws, Galois connections, order dual constructions, product/Pi instances, and proof that `Prop` forms a Heyting algebra |
| Boundary.lean | Co-Heyting boundary operator `∂ a = a ⊓ ￢a`, proving the Leibniz rule for boundaries on infima and that boundaries are idempotent; the boundary in the co-Heyting algebra of closed sets corresponds to the topological boundary |
| Hom.lean | Heyting/co-Heyting/bi-Heyting homomorphisms (`HeytingHom`, `CoheytingHom`, `BiheytingHom`) as bounded lattice homomorphisms preserving implication/difference operations, with typeclass-based `DFunLike` design, composition operations, and proofs that order isomorphisms are automatically Heyting homomorphisms |
| Regular.lean | Heyting regular elements (elements `a` with `aᶜᶜ = a`), proving they are closed under `⊓` and `⇨`, and constructing a Boolean algebra structure on the subtype `Regular α` via a Galois insertion between regularization `a ↦ aᶜᶜ` and inclusion; enables classical logic within intuitionistic logic via double negation |

## Subdirectories

(none)

## Search Tags

Heyting-algebra co-Heyting-algebra bi-Heyting-algebra intuitionistic-logic implication complement negation difference boundary regular-elements Boolean-algebra Galois-connection distributive-lattice Brouwer Cartesian-closed-category
