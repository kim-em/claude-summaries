---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/CompleteLattice
generated: 2026-01-26T06:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# CompleteLattice

## Overview

The `CompleteLattice/` directory contains the core theory of complete lattices in Mathlib. It provides the foundational definitions of complete semilattices and complete lattices (where arbitrary suprema and infima exist), along with extensive theory for working with set suprema (`sSup`), set infima (`sInf`), indexed suprema (`iSup`), and indexed infima (`iInf`). The directory includes advanced results on complete lattice structures in specific contexts: finset-indexed operations, group operations respecting lattice structure, lexicographic orderings on Pi types, bi-Cartesian squares and multicoequalizer diagrams for categorical applications, Hausdorff's maximality principle (which underpins Zorn's lemma), and `SetLike` instances for complete sublattices.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of complete lattices: `CompleteSemilatticeSup`, `CompleteSemilatticeInf`, `CompleteLattice`, `CompleteLinearOrder` classes; defines `sSup`/`sInf` (set supremum/infimum) and `iSup`/`iInf` (indexed supremum/infimum); establishes naming conventions (biSup, biInf, iSup₂, iInf₂) |
| Basic.lean | Fundamental theory of complete lattices: basic properties of `sSup`/`sInf`/`iSup`/`iInf`, interactions with unions/intersections, monotonicity lemmas, dualization via `OrderDual`, empty set behavior (`sSup ∅ = ⊥`), singleton behavior, order isomorphisms |
| Lemmas.lean | Extended theory requiring additional dependencies: complete lattice results on specific types (Bool, Nat), expressing binary operations as indexed operations (`sup_eq_iSup`, `iSup_bool_eq`), advanced manipulation of nested suprema/infima |
| Chain.lean | Hausdorff's maximality principle: proves every chain can be extended to a maximal chain; defines `ChainClosure` (reachability from `∅` via `SuccChain` and unions), `maxChain` (explicit maximal chain construction); originally ported from Isabelle/HOL |
| Finset.lean | Lattice operations indexed by finsets: `iSup_eq_iSup_finset` (expressing arbitrary suprema as suprema over finsets), dual infimum results, handles both `Type*` and `Sort*` versions (with `PLift` for universes) |
| Group.lean | Complete lattices with compatible group operations: `iSup_mul_le` and `iInf_mul_le` for monotone multiplication, works with additive and multiplicative groups respecting lattice structure, includes nested indexed versions (`iSup₂_mul_le`) |
| PiLex.lean | Complete linear order on lexicographically ordered Pi types: shows `Πₗ i, α i` is a complete linear order when each `α i` is, requires well-founded ordering on index type `ι`, defines `sInf` via dependent recursion on index |
| SetLike.lean | `SetLike` instance for complete sublattices of `Set X`: provides convenient membership lemmas for lattice operations on sublattices (`mem_inf`, `mem_sup`, `mem_sInf`, `mem_sSup`, `mem_iInf`, `mem_iSup`) |
| MulticoequalizerDiagram.lean | Bi-Cartesian squares and multicoequalizer diagrams in lattices: defines `BicartSq` (elements forming both supremum and infimum), `MulticoequalizerDiagram` for category theory applications; intended to show these become categorical limits/colimits in `Type` |

## Subdirectories

*No subdirectories*

## Search Tags

complete-lattice supremum infimum sSup sInf iSup iInf indexed-supremum complete-semilattice complete-linear-order Hausdorff-maximality maximal-chain finset-indexed lexicographic-order pi-type group-operations complete-sublattice bicartesian-square multicoequalizer category-theory bounded-supremum bounded-infimum iSup2 iInf2 biSup biInf
