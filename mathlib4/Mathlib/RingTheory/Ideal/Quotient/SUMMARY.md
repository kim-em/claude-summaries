---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Ideal/Quotient
generated: 2026-01-26T21:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Quotient

## Overview

The `Quotient/` directory contains the theory of quotient rings by ideals. It establishes quotient rings `R ⧸ I` as both rings and `R`-modules, proves fundamental isomorphism theorems (first isomorphism theorem, Chinese remainder theorem), and develops properties of quotients including their relationship to prime and maximal ideals. The directory covers quotient construction, ring homomorphism lifting, transitivity between quotients of different ideals, finiteness and Noetherian properties, nilpotent quotients, and index calculations.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of quotient ring `R ⧸ I` via `Submodule.Quotient`, ring structure, quotient map `mk`, and `lift` operation for ring homomorphisms |
| Basic.lean | Fundamental properties of quotient rings: zero/one characterization, nontriviality, prime/maximal ideal quotients (domains and fields), and `R^n/I^n ≃ (R/I)^n` |
| Operations.lean | First isomorphism theorems (`quotientKerEquivRange`), Chinese remainder theorem (`quotientInfRingEquivPiQuotient`), quotient maps and kernel properties |
| ChineseRemainder.lean | Module version of Chinese remainder theorem for pairwise coprime ideals: surjectivity of `M → Πᵢ (R ⧸ Iᵢ) ⊗[R] M` and kernel characterization |
| Index.lean | Index calculations for ideal quotients: finite index of `I • N`, bounds on index of `I^n` via generating sets |
| Nilpotent.lean | Properties of nilpotent elements in quotient rings: radical ideal characterization via reducedness of quotient, induction principle for nilpotent ideals |
| Noetherian.lean | Preservation of Noetherian property: quotients of Noetherian rings are Noetherian |
| PowTransition.lean | Quotient maps between powers of ideals: canonical maps `R ⧸ I^m → R ⧸ I^n` for m ≥ n, used in adic completion theory |

## Subdirectories

(none)

## Search Tags

quotient-ring ideal-quotient ring-homomorphism first-isomorphism-theorem Chinese-remainder-theorem quotient-map lift kernel prime-ideal maximal-ideal field division-ring domain quotient-module tensor-product coprime-ideals nilpotent radical reduced Noetherian finite-index adic-completion power-transition factor
