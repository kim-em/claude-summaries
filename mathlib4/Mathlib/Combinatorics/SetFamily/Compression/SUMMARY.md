---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SetFamily/Compression
generated: 2025-12-08T08:00:04Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Compression

## Overview

The `Compression/` directory implements compression operations on set families that reduce shadow sizes, which are fundamental tools for proving extremal combinatorics results like the Kruskal-Katona theorem. It contains two types of compressions: down-compression (removing elements from sets) and UV-compression (moving elements from one position to another in a lattice-theoretic sense). Both operations are idempotent, size-preserving, and the UV-compression is the key ingredient for proving that initial segments of colex order minimize shadow size.

## Key Files

| File | Purpose |
|------|---------|
| Down.lean | Down-compression: removes element `a` from sets in family `𝒜` when resulting set not already present; defines nonMemberSubfamily (sets without `a`) and memberSubfamily (image of sets with `a` after removing it); proves compression is idempotent, preserves cardinality, and provides induction principles (memberFamily_induction_on and family_induction_on) for reasoning about finset families by splitting into member/non-member subfamilies; notation `𝓓 a 𝒜` |
| UV.lean | UV-compression: replaces element `a` by `(a ⊔ u) \ v` when `a` and `u` are disjoint and `v ≤ a` (moving from `v` to `u`); works in generalized Boolean algebras; proves compression is injective on moved elements, idempotent, cardinality-preserving; main theorem shadow_compression_subset_compression_shadow shows UV-compression reduces shadow size when certain sub-compressions are already applied; card_shadow_compression_le is the key fact for Kruskal-Katona proof; notation `𝓒 u v 𝒜` |

## Subdirectories

*(none)*

## Search Tags

compression down-compression uv-compression set-family shadow extremal-combinatorics kruskal-katona colex member-subfamily boolean-algebra lattice idempotent cardinality-preserving induction finset-family generalized-boolean-algebra disjoint shadow-reduction
