---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/SimplexCategory/GeneratorsRelations
generated: 2025-12-04T08:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# GeneratorsRelations

## Overview

The `GeneratorsRelations/` directory provides the presentation of the simplex category by generators (face maps δ and degeneracy maps σ) and relations (the simplicial identities). It introduces `SimplexCategoryGenRel` as the free category on these generators modulo the simplicial relations, establishes induction principles for reasoning about morphisms and objects, proves every morphism admits an epi-mono factorization (as P_σ followed by P_δ), and develops normal form theory for morphisms via admissible lists. This is a crucial step toward proving the canonical functor `toSimplexCategory : SimplexCategoryGenRel ⥤ SimplexCategory` is an equivalence.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: FreeSimplexQuiver with generators δ (face maps) and σ (degeneracy maps), homRel encoding five simplicial identities, SimplexCategoryGenRel as quotient category, induction principles (hom_induction, hom_induction', rec), canonical functor toSimplexCategory, and proofs of simplicial identities in the generators-and-relations setting |
| EpiMono.lean | Epi-mono factorization theory: proves δ maps are split monomorphisms and σ maps are split epimorphisms, introduces morphism properties P_δ (compositions of faces) and P_σ (compositions of degeneracies), and main theorem exists_P_σ_P_δ_factorization showing every morphism decomposes uniquely as P_σ followed by P_δ |
| NormalForms.lean | Normal form theory: defines admissible lists (strictly increasing sequences [i₀,...,iₙ] with iₖ ≤ m+k), simplicialInsert operation for building normal forms via simplicial relations, standardσ construction mapping admissible lists to canonical P_σ morphisms, simplicialEvalσ evaluation function, and theorem exists_normal_form_P_σ showing every P_σ morphism has a unique admissible list representation |

## Subdirectories

*(No subdirectories)*

## Search Tags

simplex-category generators-relations simplicial-identities face-maps degeneracy-maps free-category quotient-category induction-principles epi-mono-factorization split-epimorphism split-monomorphism normal-forms admissible-lists simplicial-insert categorical-presentation morphism-properties
