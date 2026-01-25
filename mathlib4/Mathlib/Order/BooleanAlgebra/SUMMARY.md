---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/BooleanAlgebra
generated: 2026-01-25T19:45:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 3
subdirs_count: 0
---

# BooleanAlgebra

## Overview

The `BooleanAlgebra/` directory contains the foundational theory of Boolean algebras and generalized Boolean algebras in Mathlib. It defines the typeclass hierarchy starting from generalized Boolean algebras (distributive lattices with bottom and relative complement `\`) through full Boolean algebras (bounded distributive lattices with complement `ᶜ`), and provides comprehensive API for working with complements, set differences, and Heyting implications. The directory includes core definitions, basic lemmas about Boolean operations, and the concrete Boolean algebra instance for `Set α` that serves as the prototypical example of the theory.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass definitions: `GeneralizedBooleanAlgebra` (distributive lattice with `⊥` and relative complement `\`) and `BooleanAlgebra` (adds `⊤` and absolute complement `ᶜ`); includes instances for `Prop`, `Bool`, and `PUnit`; provides alternative constructor from complemented lattices |
| Basic.lean | Extensive API for generalized Boolean algebras and Boolean algebras: lemmas about `sdiff` (`\`) operations, complement properties (involution, monotonicity, De Morgan laws), disjointness, codisjointness, Heyting implication (`⇨`), product and Pi instances, and pullback constructions via injective functions |
| Set.lean | Boolean algebra instance for `Set α` proving that sets form a Boolean algebra under union, intersection, and complement; extensive lemmas about set difference and complement including `diff_eq_compl_inter`, `compl_compl`, `subset_compl_comm`, singleton complements, and the `Set.ite` conditional operation for sets |

## Subdirectories

(none)

## Search Tags

Boolean-algebra generalized-Boolean-algebra complement sdiff relative-complement Heyting-algebra biheying-algebra distributive-lattice bounded-order compl set-difference set-complement De-Morgan disjoint codisjoint himp Heyting-implication Stone
