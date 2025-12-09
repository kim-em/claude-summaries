---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/FunLike
generated: 2025-12-09T06:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 4
subdirs_count: 0
---

# FunLike

## Overview

The `FunLike/` directory defines the foundational typeclass infrastructure for function-like structures in mathlib4. It provides `DFunLike` (dependent function-like) and `FunLike` (non-dependent function-like) typeclasses that enable types to be coerced to functions with an injective coercion. This design pattern is used throughout mathlib for homomorphisms, embeddings, and isomorphisms (such as `MonoidHom`, `LinearMap`, `RelEmbedding`, `MonoidEquiv`), allowing polymorphic operations over function-like types while maintaining extensionality and providing automatic `CoeFun` instances. The directory includes specialized refinements for embeddings (`EmbeddingLike` for injective function-like types) and equivalences (`EquivLike` for bijective function-like types), along with finiteness results showing that function-like types are finite when their domain and codomain are finite.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `DFunLike` and `FunLike` typeclasses with injective coercion to (dependent) functions; provides `CoeFun` instances, extensionality lemmas, and comprehensive documentation on the typeclass design pattern for morphisms |
| Embedding.lean | `EmbeddingLike` typeclass for function-like structures with injective coercions (e.g., `RelEmbedding`); extends `FunLike` with injectivity requirement and provides lemmas for composition and application equality |
| Equiv.lean | `EquivLike` typeclass for function-like structures with bijective coercions (e.g., `MonoidEquiv`, `LinearEquiv`); provides both forward and inverse coercions with left/right inverse proofs, automatic `FunLike` and `EmbeddingLike` instances, and extensionality for isomorphisms |
| Fintype.lean | Finiteness results for `DFunLike` and `FunLike` types: `fintype` instances and `finite` theorems showing function-like types are finite when domain and codomain are finite; includes `DecidableEq` instance for finite function-like types |

## Subdirectories

*(No subdirectories)*

## Search Tags

funlike dfunlike function-like typeclass coercion homomorphisms embeddings equivalences isomorphisms extensionality injective-coercion morphisms monoidhom linearmap relembedding monoidequiv linearequiv finite-functions
