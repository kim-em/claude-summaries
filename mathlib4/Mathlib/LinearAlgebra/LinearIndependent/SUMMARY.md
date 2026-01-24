---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/LinearIndependent
generated: 2026-01-25T22:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# LinearIndependent

## Overview

The `LinearIndependent/` directory contains the core formalization of linear independence in mathlib4. It defines linear independence as injectivity of the linear combination map, provides numerous equivalent characterizations (kernel conditions, explicit linear combinations, fintype variants), and establishes fundamental properties including injectivity of linearly independent families, scalar tower restrictions, composition lemmas, and specialized tests for specific constructions (pairs, options, fin-indexed families). The directory includes proofs over semirings (avoiding kernel arguments where possible), rings (with kernel characterizations), and division rings (with span-based characterizations), plus maximal linear independence, extension theorems, and Dedekind's linear independence of characters.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `LinearIndependent R v` as injectivity of `Finsupp.linearCombination R v`, `LinearIndepOn R v s` for indexed families, canonical representation `LinearIndependent.repr`, maximal linear independence, and multiple equivalent characterizations across semirings (iffₛ variants), linearly ordered semirings (iffₒₛ variants), and rings (kernel-based iff). Includes delaborator for pretty-printing subtype-indexed families |
| Basic.lean | Fundamental consequences and specialized tests: scalar restriction (`restrict_scalars`, `restrict_scalars'`), image preservation under injective/surjective maps (`map_injOn`, `map_of_injective_injectiveₛ`, `map_of_surjective_injectiveₛ`), span disjoint properties, union operations (`sum_type`, `union`, `inl_union_inr`), maximal extension (`exists_maximal_linearIndepOn'`), pair tests, finite-indexed tests, Dedekind's linear independence of monoid/algebra homomorphisms (`linearIndependent_monoidHom`, `linearIndependent_algHom_toLinearMap`) |
| Lemmas.lean | Advanced properties requiring more theory: option/fin constructions (`linearIndependent_option`, `linearIndependent_fin_cons`, `linearIndependent_fin_succ`), insertion lemmas for division rings (`LinearIndepOn.insert`, `linearIndepOn_insert`), extension theorems (`exists_linearIndepOn_extension`, `LinearIndepOn.extend`), span exchange properties (`mem_span_insert_exchange`), finiteness results (`exists_of_linearIndepOn_of_finite_span`, `exists_finite_card_le_of_finite_of_linearIndependent_of_span`), pair manipulation lemmas with scalars (`pair_add_smul_add_smul_iff`, `pair_add_right_iff`), bijective characterization from spanning and independence |

## Subdirectories

(No subdirectories)

## Search Tags

linear-independence linear-dependence linearly-independent linearly-dependent finsupp-linear-combination injective-linear-map kernel maximal-linear-independence dedekind-independence extension-theorem span vector-spaces modules semirings rings division-rings fin-indexed option-indexed pairs sums unions
