---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Perfectoid
generated: 2026-02-01T10:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 3
subdirs_count: 0
---

# Perfectoid

## Overview

This folder contains foundational constructions for perfectoid theory and p-adic Hodge theory in Mathlib. It implements the tilting and untilting operations that relate a p-adically complete ring R to its tilt R♭ (the perfection of R/p), along with Fontaine's θ map from Witt vectors 𝕎(R♭) to R, and the de Rham period rings 𝔹_dR⁺ and 𝔹_dR. These are key objects in modern arithmetic geometry, particularly for studying p-adic representations of Galois groups.

## Key Files

| File | Purpose |
|------|---------|
| Untilt.lean | Defines the untilt function from PreTilt O p (the tilt of a p-adically complete ring O) back to O itself; proves the untilt is multiplicative and that composing with mod p equals the zeroth perfection component |
| FontaineTheta.lean | Constructs Fontaine's θ map: 𝕎(R♭) →+* R as a limit of maps through R/p^n; proves θ sends Teichmüller representatives to untilts and is surjective when Frobenius is surjective on R/p |
| BDeRham.lean | Defines the de Rham period rings 𝔹_dR⁺ (adic completion of 𝕎(R♭)[1/p] at ker θ) and 𝔹_dR (localization inverting ker θ generators); follows Scholze's generalized approach for perfectoid rings |

## Subdirectories

(none)

## Search Tags

perfectoid tilt untilt Fontaine theta p-adic Hodge theory de Rham period ring Witt vectors pretilt frobenius adic completion B_dR arithmetic geometry Galois representations
