---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/LegendreSymbol/QuadraticChar
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# QuadraticChar

## Overview

The `QuadraticChar/` directory provides the formalization of quadratic characters on finite fields, which are multiplicative characters that determine whether elements are quadratic residues. The main content includes the definition of the quadratic character as a map to ℤ (taking values 0, 1, -1), proofs of its multiplicativity and basic properties, computation via Euler's criterion (raising to the power (card F / 2)), and special value theorems relating quadratic characters to χ₄ and χ₈ characters. This theory connects quadratic residuosity in finite fields to modular arithmetic via character relations, with applications to determining when specific elements like -1, 2, -2, and odd primes are squares in finite fields.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core quadratic character definition on finite fields, multiplicative character structure, dichotomy theorem (value is 0, 1, or -1), computation via Euler's criterion (a^(card/2)), special values for -1 (via χ₄), counting square roots, sum-to-zero property for odd characteristic |
| GaussSum.lean | Special values of quadratic character via Gauss sum theory: values at 2 (via χ₈) and -2 (via χ₈'), criteria for when 2/-2 are squares based on card F mod 8, reciprocity-style theorem relating quadraticChar F (card F') and quadraticChar F' (card F), determining when odd primes are squares in F |

## Subdirectories

*(No subdirectories)*

## Search Tags

quadratic-character finite-field multiplicative-character euler-criterion quadratic-residue isSquare chi4 chi8 gauss-sum special-values card-sqrts quadratic-reciprocity zmod odd-prime characteristic ring-char
