---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/AffineSpace/AffineSubspace
generated: 2026-01-25T22:52:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# AffineSubspace

## Overview

The `AffineSubspace/` directory contains the core theory of affine subspaces in mathlib4. It provides the fundamental definitions (`Defs.lean`) and additional properties (`Basic.lean`) of affine subspaces, which are subsets of affine spaces that preserve the affine structure. Key concepts include the `AffineSubspace` type (subsets closed under affine combinations), the `direction` of a subspace (associated vector submodule), `affineSpan` (smallest affine subspace containing a set), complete lattice structure on affine subspaces, and operations like `map`/`comap` for affine maps. The directory also develops the theory of parallel affine subspaces and provides extensive lemmas relating affine subspaces to their directions and spans.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `AffineSubspace` structure (carrier set with `smul_vsub_vadd_mem` closure), `vectorSpan` (submodule spanned by pairwise differences), `spanPoints` helper, `affineSpan` (Galois insertion with sets), `direction` of subspaces, `mk'` constructor from point and direction, complete lattice structure (⊤, ⊥, ⊔, ⊓, sSup, sInf) |
| Basic.lean | Extended theory: `toAddTorsor` instance making nonempty subspaces into torsors over their direction, `subtype` embedding, `lineMap` membership lemmas, affine span of singletons and pairs, direction of suprema and infima, `map`/`comap` for affine maps with Galois connection, `Parallel` relation (s₁ ∥ s₂ when one is translation of other) with equivalence properties |

## Subdirectories

*(none)*

## Search Tags

affine-subspace affine-span vector-span direction affine-combinations spanPoints mk' complete-lattice affine-map-comap parallel-subspaces galois-connection line-affine-span add-torsor-structure affine-independence vectorSpan affineSpan
