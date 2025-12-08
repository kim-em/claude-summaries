---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SetFamily
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 9
subdirs_count: 1
---

# SetFamily

## Overview

The `SetFamily/` directory provides theory for families of finite sets, including fundamental extremal combinatorics results. It covers shadows (removing elements from sets), shattering (VC-dimension theory), intersecting families (pairwise non-disjoint collections), and major theorems like Kruskal-Katona (bounds on shadow sizes via colex initial segments), Lubell-Yamamoto-Meshalkin/Sperner (antichain size bounds), Harris-Kleitman (correlation of upper/lower sets), Ahlswede-Zhang (identity for truncated unions), and Erdős-Ko-Rado (maximum intersecting family size).

## Key Files

| File | Purpose |
|------|---------|
| AhlswedeZhang.lean | Ahlswede-Zhang identity for set families: proves that sum of weighted truncated infima equals 1, with truncatedSup/truncatedInf operations on lattices; sharpens LYM inequality by making explicit the correction term; includes proofs that initial segments minimize this sum |
| FourFunctions.lean | Four Functions Theorem (Ahlswede-Daykin inequality): if f₁(a)·f₂(b) ≤ f₃(a⊓b)·f₄(a⊔b) pointwise, then (∑f₁)·(∑f₂) ≤ (∑f₃)·(∑f₄) on set families; uses Birkhoff representation and induction on ground set size; includes corollaries: Daykin inequality, Holley inequality, Fortuin-Kastelyn-Ginibre (FKG) inequality, and Marica-Schönheim inequality |
| HarrisKleitman.lean | Harris-Kleitman inequality: proves that lower sets (or upper sets) correlate in uniform measure on finsets; for lower sets 𝒜 and ℬ, shows \|𝒜\|·\|ℬ\| ≤ 2^n·\|𝒜 ∩ ℬ\|; uses induction via member/non-member subfamilies with respect to elements |
| Intersecting.lean | Intersecting families (pairwise non-disjoint sets): defines Set.Intersecting predicate, proves maximal intersecting families are upper sets, shows intersecting families can contain at most half the elements (a and aᶜ cannot both be in), and establishes that maximal intersecting families have size exactly 2^(n-1) in nontrivial Boolean algebras |
| Kleitman.lean | Kleitman's bound on intersecting families: proves that k intersecting families cover at most 2^n - 2^(n-k) sets; uses Harris-Kleitman inequality and induction on the number of families; shows each additional intersecting family takes at most half of remaining uncovered sets |
| KruskalKatona.lean | Kruskal-Katona theorem: proves minimum shadow size is achieved by initial segments of colex order; shows shadow of initial segment is also initial segment; includes iterated version and Lovasz formulation (if \|𝒜\| ≥ (k choose r), then \|∂^i 𝒜\| ≥ (k choose (r-i))); culminates in Erdős-Ko-Rado theorem (maximum r-uniform intersecting family has size at most (n-1 choose r-1) when r ≤ n/2) |
| LYM.lean | Lubell-Yamamoto-Meshalkin (LYM) inequality and Sperner's theorem: proves local LYM (shadow takes greater proportion of its layer), global LYM (sum of layer densities ≤ 1 for antichains), and Sperner's theorem (maximum antichain size is (n choose n/2)); uses "falling" construction to iteratively bound contributions from each layer |
| Shadow.lean | Shadow operations on set families: defines shadow ∂𝒜 (sets obtained by removing one element) and upShadow ∂⁺𝒜 (sets obtained by adding one element); provides membership characterizations via subset relations and cardinality; proves shadows of r-sets are (r-1)-sets; includes iterated shadows with k-fold removal/addition |
| Shatter.lean | Shattering and VC-dimension: defines Shatters predicate (all subsets of s obtainable as s ∩ t for t ∈ 𝒜), shatterer (family of all shattered sets), and vcDim (maximum size of shattered set); proves Pajor and Sauer-Shelah lemmas bounding shatterer size; shows compressions preserve and decrease VC-dimension; used in statistical learning theory |

## Subdirectories

- [ ] `Compression/` - Compression operations on set families (pending)

## Search Tags

set-family extremal-combinatorics shadow colex kruskal-katona sperner lym lubell-yamamoto-meshalkin antichain intersecting harris-kleitman ahlswede-zhang four-functions fkg daykin holley marica-schonheim erdos-ko-rado vc-dimension shattering sauer-shelah vapnik-chervonenkis combinatorial-optimization
