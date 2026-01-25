---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Transcendental/Liouville
generated: 2026-01-25T22:15:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 5
subdirs_count: 0
---

# Liouville

## Overview

This directory contains a comprehensive formalization of Liouville numbers and Liouville's theorem in Lean 4. The main result is that all Liouville numbers are transcendental. The implementation includes the classical definition of Liouville numbers, the construction of explicit Liouville constants, a generalized notion of Liouville numbers with arbitrary exponents, measure-theoretic properties showing the set has Lebesgue measure zero, and topological results showing the set is dense and residual (a dense Gδ set). This provides both the classical transcendence result and modern measure/topology perspectives on these numbers.

## Key Files

| File | Purpose |
|------|---------|
| `Basic.lean` | Core definition of Liouville numbers and proof of Liouville's theorem (Liouville numbers are transcendental); includes technical lemmas about polynomial evaluation and Diophantine approximation |
| `LiouvilleNumber.lean` | Construction of explicit Liouville constants indexed by natural numbers m ≥ 2, defined as the series Σ(1/m^(i!)); proves these are transcendental |
| `LiouvilleWith.lean` | Generalized Liouville condition with arbitrary exponents p; a number is LiouvilleWith p if it can be approximated by rationals a/b with error < C/b^p for infinitely many denominators |
| `Measure.lean` | Measure-theoretic properties: proves the set of Liouville numbers (with exponent > 2) has Lebesgue measure zero; shows residual and ae volume filters are disjoint |
| `Residual.lean` | Topological properties: proves the set of Liouville numbers is a dense Gδ set (residual set); establishes the set as comeager in the reals |

## Subdirectories

No subdirectories.

## Search Tags

liouville-numbers transcendental liouville-theorem diophantine-approximation irrationality-measure algebraic-numbers liouville-constant gδ-set residual measure-zero dense-set baire-category polynomial-evaluation continued-fractions
