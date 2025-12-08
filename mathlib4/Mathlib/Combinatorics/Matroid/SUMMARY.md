---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Matroid
generated: 2025-12-08T07:43:53Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 10
subdirs_count: 2
---

# Matroid

## Overview

The `Matroid/` directory contains a comprehensive formalization of matroid theory, a combinatorial abstraction of linear independence that unifies concepts from graph theory, discrete optimization, and algebraic geometry. Matroids are defined axiomatically in terms of bases (maximal independent sets), following the B-matroid definition that generalizes naturally to infinite ground sets. The implementation uses `ℕ∞`-valued cardinality to handle both finite and infinite matroids uniformly, with special API for finite cases via typeclasses. Core concepts include independence, bases, circuits (minimal dependent sets), closure (combinatorial span), loops (zero elements), coloops (bridges), duality, and rank functions satisfying submodularity.

## Key Files

| File | Purpose |
|------|---------|
| Init.lean | Declares the `Matroid` Aesop rule set for the `aesop_mat` tactic; must be in separate file for visibility |
| Basic.lean | Core matroid definition via base axioms, independent sets (`M.Indep`), dependent sets (`M.Dep`), bases of sets (`M.IsBasis`), finiteness predicates (`M.Finite`, `RankFinite`, `Finitary`), and fundamental API; uses B-matroid axioms allowing infinite ground sets with equicardinality via `Set.encard : ℕ∞` |
| IndepAxioms.lean | Alternative matroid constructions via independence predicates; defines `IndepMatroid` structure with nontriviality, monotonicity, and augmentation axioms; includes simplified axiom sets for finitary, bounded-rank, finite ground sets, and finset-based matroids; uses Zorn's lemma for infinite cases |
| Circuit.lean | Circuits (minimal dependent sets); fundamental circuits (`fundCircuit M e I` is unique circuit in `insert e I` for independent `I` with `e ∈ closure I`); circuit elimination axioms; cocircuits (circuits in dual, equivalently `M.E \ C` is hyperplane); proves `ext_isCircuit` (matroids determined by circuits) and finitary characterization via finite circuits |
| Closure.lean | Flats (combinatorial subspaces) and closure operator (`M.closure : Set α → Set α`); spanning sets (closure equals ground set); defines `M.subtypeClosure` as `ClosureOperator` on subtype `↑(Iic M.E)`; implementation choice: `M.closure X = M.closure (X ∩ M.E)` ensures `M.closure X ⊆ M.E` unconditionally at cost of `X ⊆ M.closure X` requiring `X ⊆ M.E` |
| Loop.lean | Loops (`e ∈ M.closure ∅`, equivalently `{e}` is dependent/circuit) and nonloops; coloops (loops in dual, equivalently in every base, or `M.E \ {e}` is nonspanning); equivalences via `isLoop_tfae` and `isColoop_tfae`; `M.removeLoops` restriction to nonloop elements; `M.Loopless` typeclass |
| Dual.lean | Matroid duality via base complement: `M✶.IsBase B ↔ M.IsBase (M.E \ B)`; defines `dualIndepMatroid` structure and `M.Coindep X` abbreviation for `M✶.Indep X` (subsets of base complements); duality is involutive and preserves representability/connectivity |
| Map.lean | Maps between matroids via functions: `comap N f` (preimage matroid with independence requiring injectivity and image-independence), `map M f` (image matroid, isomorphic to source), variants for embeddings (`mapEmbedding`, `mapSetEmbedding`) and equivalences (`mapEquiv`, `mapSetEquiv`); isomorphisms represented as maps |
| Sum.lean | Direct sum constructions: `sigma M` for indexed families on sigma-types `(Σ i, α i)`, `sum' M` for families on product types `ι × α`, `disjointSigma M h` for families with disjoint ground sets as `Matroid α`, `sum M N` for pairs on `α ⊕ β`, `disjointSum M N h` for disjoint pairs; independent sets are unions of summand-independent sets |
| Constructions.lean | Elementary matroids: `emptyOn α` (empty ground set), `loopyOn E` (all loops, only base is `∅`), `freeOn E` (ground set is only base), `uniqueBaseOn I E` (single base `I ⊆ E`); bootstrapped via duality and restriction to avoid axiom certification |

## Subdirectories

- [ ] `Minor/` - Matroid minors (deletion, contraction, restriction operations) (pending)
- [ ] `Rank/` - Rank functions: `ℕ∞`-valued (`eRank`, `eRk`), finite rank, cardinal-valued variants (pending)

## Search Tags

matroid combinatorics linear-algebra independence basis circuit cocircuit closure flat spanning loop coloop nonloop duality rank submodularity finitary b-matroid infinite-matroid graph-theory discrete-optimization galois-insertion aesop-tactic
