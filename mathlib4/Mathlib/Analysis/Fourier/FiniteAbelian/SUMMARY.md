---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Fourier/FiniteAbelian
generated: 2025-12-05T07:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# FiniteAbelian

## Overview

The `FiniteAbelian/` directory develops Fourier analysis on finite abelian groups, focusing on the orthogonality properties of characters and Pontryagin duality. It proves that characters of a finite abelian group are orthogonal (with weighted inner product equal to 1 for identical characters and 0 otherwise), that there are at most as many characters as group elements, and that finite abelian groups are canonically isomorphic to their double dual (the space of characters of characters). The theory is first established for `ZMod n` and then extended to all finite abelian groups via the Structure Theorem.

## Key Files

| File | Purpose |
|------|---------|
| Orthogonality.lean | Proves orthogonality of characters: `⟪ψ₁, ψ₂⟫ₙ = if ψ₁ = ψ₂ then 1 else 0`; shows characters are linearly independent over ℂ; proves `card (AddChar G R) ≤ card G`; establishes expectation formulas `𝔼 a, ψ a = if ψ = 0 then 1 else 0` |
| PontryaginDuality.lean | Proves Pontryagin duality for finite abelian groups: any finite abelian group is canonically isomorphic to its double dual `AddChar (AddChar α ℂ) ℂ`; defines indexing of `ZMod n` characters via `AddChar.zmod n x = e^(2πixy/n)`; shows `card (AddChar α ℂ) = card α`; constructs `complexBasis` making characters a basis of `α → ℂ` |

## Subdirectories

None - this is a leaf directory.

## Search Tags

fourier-analysis finite-abelian-groups character-theory pontryagin-duality orthogonality-relations additive-characters zmod-characters double-dual hilbert-basis linear-independence complex-characters circle-characters weighted-inner-product structure-theorem
