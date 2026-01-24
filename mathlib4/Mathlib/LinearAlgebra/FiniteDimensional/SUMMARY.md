---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/FiniteDimensional
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# FiniteDimensional

## Overview

The `FiniteDimensional/` directory contains the core theory of finite-dimensional vector spaces over division rings. It establishes the fundamental `FiniteDimensional K V` typeclass (defined as `Module.Finite K V`), proves equivalence between multiple characterizations (finite basis, finitely generated, Noetherian), and develops properties including dimension formulas, preservation under constructions (submodules, quotients, linear equivalences), and structural theorems like rank-nullity. The files are organized hierarchically: definitions and basic typeclass instances, fundamental properties and dimension calculations, then advanced lemmas requiring heavier imports.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `FiniteDimensional K V` typeclass as `Module.Finite`, equivalence proofs between characterizations (finite basis via `fintypeBasisIndex`, finitely generated, Noetherian), basic instances (pi types, submodules, quotients), constructors from positive finrank (`of_finrank_pos`, `of_finrank_eq_succ`), and preservation under linear maps (injective, surjective, tower law for field extensions) |
| Basic.lean | Fundamental properties of finite-dimensional spaces: submodule dimension bounds (`Submodule.eq_top_of_finrank_eq`, `finrank_lt`), dimension arithmetic for submodule operations (inf, sup, finset sup), one-dimensional basis construction (`basisSingleton`), rank-nullity theorem (`finrank_range_add_finrank_ker`), relations between linear independence and cardinality, and existence of nontrivial relations when finrank constraint violated |
| Lemmas.lean | Advanced theorems requiring heavier imports: dimension formulas for submodule lattice operations (`finrank_sup_add_finrank_inf_eq`, `finrank_add_finrank_le_of_disjoint`), complement characterizations (`eq_top_of_disjoint`, `isCompl_iff_disjoint`), quotient isomorphisms (`LinearEquiv.quotEquivOfEquiv`, `LinearEquiv.quotEquivOfQuotEquiv`), and kernel non-triviality from dimension constraints (`ker_ne_bot_of_finrank_lt`) |

## Subdirectories

(none)

## Search Tags

finite-dimensional vector-spaces finrank dimension typeclass division-ring basis noetherian finitely-generated rank-nullity submodule quotient linear-equiv linear-map kernel range complement disjoint isomorphism tower-law field-extension cardinality linear-independence
