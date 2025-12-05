---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/FunctionalSpaces
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# FunctionalSpaces

## Overview

The `FunctionalSpaces/` directory contains the formalization of the Gagliardo-Nirenberg-Sobolev inequality, a fundamental result in functional analysis. This inequality bounds the Lᵖ norm of compactly-supported C¹ functions by the Lᵖ norm of their derivatives, up to dimension-dependent constants. The proof uses a sophisticated inductive argument called the "grid-lines lemma" that manipulates iterated integrals and applies Hölder's inequality.

## Key Files

| File | Purpose |
|------|---------|
| SobolevInequality.lean | Proves the Gagliardo-Nirenberg-Sobolev inequality for continuously differentiable compactly-supported functions on finite-dimensional normed spaces; main results include bounds for 1 ≤ p < n with q⁻¹ = p⁻¹ - n⁻¹, as well as specialized versions for Hilbert and Banach space codomains; features the "grid-lines lemma" (a complex inductive argument using iterated integrals and Hölder's inequality) as the key technical tool |

## Subdirectories

None.

## Search Tags

functional-analysis sobolev-inequality gagliardo-nirenberg-sobolev derivatives lp-norms normed-spaces haar-measure holder-inequality compact-support grid-lines-lemma iterated-integrals finite-dimensional-spaces banach-spaces hilbert-spaces frechet-derivative continuous-differentiable measure-theory analysis
