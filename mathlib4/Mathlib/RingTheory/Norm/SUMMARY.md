---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Norm
generated: 2026-02-01T12:00:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 3
subdirs_count: 0
---

# Norm

## Overview

This folder defines and develops the algebra norm for finite ring and field extensions. The norm of an element `s` in an `R`-algebra `S` is defined as the determinant of the left multiplication map `(*) s : S →ₗ[R] S`. The implementation is designed to be maximally general, with assumptions about fields or finite extensions added to individual lemmas as needed. Key results include the relationship between norms and minimal polynomial roots, transitivity of norms through towers of extensions, and the product formula over embeddings for separable extensions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Algebra.norm` as the determinant of left multiplication; proves `norm_algebraMap` gives `x ^ finrank` for base ring elements |
| Basic.lean | Fundamental properties including `norm_zero`, `norm_eq_zero_iff` for domains, `norm_inv`, power basis formulas relating norm to minimal polynomial roots, and norm preservation under algebra equivalences |
| Transitivity.lean | Proves the transitivity theorem `norm R (norm S a) = norm R a` for towers R/S/A of finite free extensions; includes Silvester's block matrix determinant theorem and the product formula `norm K x = prod of embeddings` for separable extensions |

## Subdirectories

(none)

## Search Tags

algebra-norm field-norm determinant ring-extension field-extension power-basis minimal-polynomial roots-of-polynomial separable-extension galois-extension transitivity embedding algebra-tower left-multiplication block-matrix finrank norm-zero norm-inv
