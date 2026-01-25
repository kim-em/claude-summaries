---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/ArithmeticFunction
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# ArithmeticFunction

## Overview

The `ArithmeticFunction/` directory provides a comprehensive framework for arithmetic functions (functions `ℕ → R` that map 0 to 0) equipped with Dirichlet convolution as multiplication. This forms the Dirichlet ring of arithmetic functions. The directory includes fundamental arithmetic functions (Möbius μ, von Mangoldt Λ, zeta ζ, Carmichael λ), divisor sums (σ), and prime factor counting functions (ω, Ω), along with their algebraic properties, multiplicativity theory, and classical identities like Möbius inversion.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of arithmetic functions, Dirichlet convolution, multiplicative functions, and ring structure |
| Moebius.lean | Möbius function μ and Möbius inversion formulas for sums and products |
| VonMangoldt.lean | Von Mangoldt function Λ with classical summation property ∑_{d\|n} Λ(d) = log n |
| Zeta.lean | Zeta function ζ (constant 1 on positive naturals) and pointwise operations (pmul, pdiv, ppow) |
| Carmichael.lean | Carmichael function λ (reduced totient) defined as exponent of (ZMod n)ˣ with prime power formulas |
| Misc.lean | Divisor sum function σ, prime factor counts ω and Ω, identity and power functions, with multiplicativity proofs |

## Subdirectories

(none)

## Search Tags

arithmetic-functions dirichlet-convolution multiplicative-functions mobius-function von-mangoldt zeta-function carmichael-function divisor-sums sigma-function mobius-inversion prime-factors totient
