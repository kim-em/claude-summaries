---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic/Embedding
generated: 2026-01-25T18:42:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Embedding

## Overview

The `Embedding/` directory defines the core type `Function.Embedding` (notation `α ↪ β`) for bundled injective functions, a fundamental building block used throughout mathlib to express embeddings between types. Basic.lean provides the primary infrastructure including the embedding structure itself, basic operations (identity, composition, congruence), constructions for product/sum/sigma types and function spaces, and specialized embeddings like subtype inclusions and quotient projections. Set.lean adds set-theoretic operations including codomain restriction, set image embeddings, subset inclusions, and embeddings for disjoint unions of sets.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Function.Embedding α β` (notation `α ↪ β`) as bundled injective functions with `toFun : α → β` and injectivity proof; includes FunLike/EmbeddingLike instances, basic operations (refl, trans, congr), conversions to/from Equiv, constructions for Option/Subtype/products/sums/sigma types/pi types, arrow congr embeddings (left/right), setValue for point modification, and specialized embeddings (some, quotientOut, punit); establishes fundamental embedding algebra with composition, identity, and extensionality |
| Set.lean | Set-theoretic embedding operations: `optionElim` for extending embeddings with a point outside the range, `optionEmbeddingEquiv` characterizing Option embeddings as sigma over complement, `codRestrict` for restricting codomain to a subset, `Embedding.image` mapping sets through embeddings, `Set.embeddingOfSubset` for subset inclusions, `subtypeOrEquiv` for splitting disjunctive subtypes, and `sumSet`/`sigmaSet` embeddings for disjoint unions; requires Set.Image, Pairwise relations |

## Subdirectories

(No subdirectories)

## Search Tags

embedding injective-functions bundled-functions function-embedding basic-algebra composition identity subtype option product sum sigma pi-types set-operations mathlib lean4 type-theory
