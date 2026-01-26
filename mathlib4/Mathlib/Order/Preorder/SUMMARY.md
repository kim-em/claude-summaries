---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Preorder
generated: 2026-01-26T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Preorder

## Overview

The `Preorder/` subdirectory contains specialized theory for preorders, partial orders, and linear orders that doesn't fit in the main hierarchy files. This includes chain theory (comparable element sets and maximal chains/flags), finiteness results for preordered sets (existence of minimal/maximal elements in finite sets), and pointwise order structures on finitely supported functions (Finsupp).

## Key Files

| File | Purpose |
|------|---------|
| Chain.lean | Chains and flags: `IsChain` (sets of comparable elements), `SuperChain`, `IsMaxChain`, `Flag` (maximal chains as a type with SetLike instance), chain operations (image, preimage, union under order embeddings/isomorphisms), SuccChain construction for extending chains; originally ported from Isabelle/HOL's Zorn theory |
| Finite.lean | Finite preorders and finite sets: existence of minimal/maximal elements in nonempty finite sets (`Finset.exists_maximal`, `Set.Finite.exists_minimal`), characterization of infinite sets via unbounded sequences (`infinite_of_forall_exists_gt`), finiteness of top/bot elements in partial orders |
| Finsupp.lean | Pointwise order on finitely supported functions: lifts order structures (Preorder, PartialOrder, SemilatticeInf, SemilatticeSup, Lattice) from `M` to `ι →₀ M`, defines `orderEmbeddingToFun` and `orderIsoFunOnFinite`, pointwise operations on support sets |

## Subdirectories

None

## Search Tags

chain maximal-chain flag IsChain IsMaxChain SuperChain SuccChain comparable-set finite-preorder minimal-element maximal-element finite-set finsupp pointwise-order order-embedding Zorn
