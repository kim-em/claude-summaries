---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Padics
generated: 2026-01-25T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 12
subdirs_count: 1
---

# Padics

## Overview

The `Padics/` directory provides a comprehensive formalization of p-adic number theory, from foundational p-adic valuations through the complete construction of p-adic numbers and their analytic theory. At the foundation, the `PadicVal/` subdirectory defines p-adic valuations on ℕ, ℤ, and ℚ, including Legendre's and Kummer's theorems relating valuations to combinatorial structures. Building on these valuations, the directory constructs the p-adic numbers `ℚ_[p]` as the Cauchy completion of `ℚ` and the p-adic integers `ℤ_[p]` as the norm-bounded subring, establishing their complete nonarchimedean field and discrete valuation ring structures. Advanced topics include Hensel's lemma for polynomial root existence, Mahler's theorem connecting continuous functions to vanishing sequences via the Mahler basis, ring homomorphisms to finite quotients `ZMod p^n`, continuous additive characters, and multiple equivalent characterizations of p-adic structures through adic completions, valued field completions, and complex extensions `ℂ_[p]`.

## Key Files

| File | Purpose |
|------|---------|
| PadicNumbers.lean | Core definition of p-adic numbers `ℚ_[p]` as Cauchy completion, p-adic norm extension, field structure, and completeness proofs |
| PadicIntegers.lean | p-adic integers `ℤ_[p]` as subtype with norm ≤ 1, proving completeness, local ring structure, and discrete valuation ring properties |
| PadicNorm.lean | p-adic norm on `ℚ` defined as `p^(-padicValRat p q)`, proving nonarchimedean absolute value properties |
| Hensel.lean | Hensel's lemma for polynomial root existence in `ℤ_[p]`, following Lewis's formal proof |
| MahlerBasis.lean | Mahler basis functions `mahler k` and Mahler's theorem: continuous functions `ℤ_[p] → E` are Banach-isomorphic to vanishing sequences |
| RingHoms.lean | Ring homomorphisms from `ℤ_[p]` to `ZMod p^n`, kernels, residue field isomorphism, and universal property as projective limit |
| AddChar.lean | Continuous additive characters of `ℤ_[p]`, bijection with topologically nilpotent elements via `κ ↦ κ(1) - 1` |
| HeightOneSpectrum.lean | Isomorphisms between adic completions `v.adicCompletion ℚ` and `ℚ_[p]`, connecting height-one spectra to prime numbers |
| WithVal.lean | Field isomorphisms between `(Rat.padicValuation p).Completion` and `ℚ_[p]`, showing equivalence of completion constructions |
| Complex.lean | p-adic complex numbers `ℂ_[p]` as completion of algebraic closure of `ℚ_[p]`, with extended norm and valuation structures |
| ProperSpace.lean | Proofs that `ℤ_[p]` is totally bounded and compact, and `ℚ_[p]` is a proper metric space |
| ValuativeRel.lean | Valuative relation instance for `ℚ_[p]`, valuation compatibility, and rank-one properties |

## Subdirectories

- [x] `PadicVal/` - p-adic valuations on ℕ, ℤ, ℚ with Legendre's and Kummer's theorems

## Search Tags

p-adic p-adic-numbers padic-integers completion cauchy-sequence nonarchimedean ultrametric discrete-valuation-ring local-ring hensel-lemma mahler-basis valuation p-adic-norm zmod ring-homomorphism additive-character adic-completion valued-field padic-complex proper-space compact totient residue-field projective-limit
