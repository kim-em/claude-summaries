---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Matroid/Rank
generated: 2025-12-08T07:46:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Rank

## Overview

The `Rank/` directory formalizes rank functions for matroids in three variations: `ℕ∞`-valued rank (`eRank`, `eRk`) providing uniform treatment of finite and infinite matroids with strong equicardinality properties; finite-rank predicates (`IsRkFinite`) characterizing sets with finite bases enabling integer arithmetic on ranks; and cardinal-valued rank (`cRank`, `cRk`) whose behavior depends on the `InvariantCardinalRank` typeclass (provably satisfied by finitary matroids, universally true under GCH). The `ℕ∞`-valued rank is the primary API, proving submodularity axioms (R1-R3) that characterize finite matroids, while cardinal rank addresses set-theoretic subtleties where basis equicardinality is ZFC-independent.

## Key Files

| File | Purpose |
|------|---------|
| ENat.lean | `ℕ∞`-valued rank functions `eRank : ℕ∞` (matroid rank) and `eRk : Set α → ℕ∞` (set rank); proves all bases have equicardinal `encard`, establishes submodularity `eRk (X ∩ Y) + eRk (X ∪ Y) ≤ eRk X + eRk Y`, dual rank formula `M✶.eRk X + M.eRank = M.eRk (M.E \ X) + X.encard`, independence characterizations via rank/cardinality equality, and construction-specific rank computations (loopy, free, map, dual) |
| Finite.lean | `IsRkFinite M X` predicate meaning all bases of `X` are finite (equivalently `(M ↾ X).RankFinite`); provides basis finiteness characterizations, closure operations preserving finite-rankness, union/intersection/insertion lemmas, and connection between finiteness and existence of finite/finset bases; enables integer arithmetic on rank in largest natural class of sets |
| Cardinal.lean | Cardinal-valued rank `cRank : Cardinal` and `cRk : Set α → Cardinal` as suprema over basis cardinalities; defines `InvariantCardinalRank` typeclass asserting `#(I \ J) = #(J \ I)` for all bases `I`, `J` of same set (ensures well-defined cardinal rank); proves finitary matroids satisfy typeclass, establishes submodularity and preservation under map/comap/restriction, and relates cardinal rank to `eRank` via `toENat`; includes detailed notes on ZFC-independence of general basis equicardinality |

## Subdirectories

(none)

## Search Tags

matroid rank erank erk crank crk rank-function submodularity finite-rank infinite-rank cardinal-rank enat-valued natural-extended cardinality basis-cardinality equicardinality independent-set finite-basis rankfinite isrkfinite invariant-cardinal-rank finitary-matroid zfc-independence axioms-r1-r2-r3 dual-rank set-theory
