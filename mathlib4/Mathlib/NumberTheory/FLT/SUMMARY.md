---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/FLT
generated: 2026-01-25T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# FLT

## Overview

The `FLT/` directory contains formalizations related to Fermat's Last Theorem (FLT), stating that `a^n + b^n = c^n` has no nontrivial natural number solutions for `n ≥ 3`. The directory includes the basic statement of FLT, complete proofs for specific exponents (n=3 and n=4), a polynomial version of FLT over fields, and the Mason-Stothers theorem (polynomial ABC theorem). While FLT in full generality remains unformalized (the proof by Wiles and Taylor-Wiles is being formalized separately at https://github.com/ImperialCollegeLondon/FLT), these files provide verified proofs of special cases and related results.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of FLT: `FermatLastTheoremWith R n` (for semiring R), `FermatLastTheoremFor n` (for ℕ), and `FermatLastTheorem` (the main statement for n≥3). Includes equivalence proofs across ℕ, ℤ, ℚ, relaxed variant FLT', reduction to coprime case, and helper lemmas for descent arguments. |
| Four.lean | Complete proof of `fermatLastTheoremFour`: FLT for n=4, showing `a^4 + b^4 ≠ c^4` for nonzero integers. Uses infinite descent via the intermediate equation `a^4 + b^4 = c^2` and Pythagorean triple classification. Also proves that FLT for all n≥3 reduces to proving it for odd primes. |
| Three.lean | Complete proof of `fermatLastTheoremThree`: FLT for n=3 using case analysis (Case 1: elementary congruences mod 9; Case 2: descent in cyclotomic ring ℤ[ζ₃]). Implements infinite descent on multiplicity of λ=ζ₃-1 via the generalized equation `a^3 + b^3 = u*c^3` in the Eisenstein integers, relying on Kummer's lemma for units. |
| MasonStothers.lean | Proof of the Mason-Stothers theorem (polynomial ABC theorem): for coprime polynomials `a, b, c` over a field with `a+b+c=0`, either `max{deg(a), deg(b), deg(c)} + 1 ≤ deg(rad(abc))` or all derivatives are zero. Based on Wronskian arguments and radical/divRadical theory. |
| Polynomial.lean | Proof of FLT for polynomials over fields: for `n≥3` not divisible by char(k), coprime nonzero polynomials satisfying `a^n + b^n = c^n` must all be constant. More generally proves the Fermat-Catalan equation `u*a^p + v*b^q + w*c^r = 0` has only constant solutions when `p,q,r≥3` with `q*r + r*p + p*q ≤ p*q*r`. Uses Mason-Stothers and descent in positive characteristic. |

## Subdirectories

None.

## Search Tags

fermat-last-theorem FLT number-theory diophantine-equations infinite-descent pythagorean-triples cyclotomic-fields eisenstein-integers mason-stothers abc-theorem polynomial-abc wiles-taylor-wiles modular-forms case-n-equals-3 case-n-equals-4 kummer-lemma coprime-reduction wronskian radical fermat-catalan
