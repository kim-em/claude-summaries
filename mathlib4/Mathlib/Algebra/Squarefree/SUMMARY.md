---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Squarefree
generated: 2025-12-04T03:53:02Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Squarefree

## Overview

The `Squarefree/` directory contains the theory of squarefree elements in monoids—elements that are not divisible by any squares except squares of units. This is a fundamental notion in multiplicative number theory and algebraic factorization theory. The single file provides comprehensive characterizations via multiplicity, irreducible factorization, radical elements, and unique factorization, with applications to GCD theory, prime power divisibility, and integer squarefreeness.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Complete squarefree element theory: core definition `Squarefree r ↔ ∀ x, x * x ∣ r → IsUnit x`, fundamental properties (units/primes/irreducibles are squarefree, squarefree preserved by divisibility), characterizations via multiplicity (`emultiplicity x r ≤ 1 ∨ IsUnit x`), irreducibles (`¬(p * p ∣ x)` for irreducible p), and radical elements (`IsRadical x ↔ Squarefree x ∨ x = 0`), multiplication theory (`Squarefree (x * y) ↔ IsRelPrime x y ∧ Squarefree x ∧ Squarefree y`), prime power divisibility lemmas for products of squarefree elements, UFD characterization (`Squarefree x ↔ Multiset.Nodup (normalizedFactors x)`), GCD preservation, and integer/natural number casting theorems |

## Subdirectories

(none)

## Search Tags

squarefree monoid multiplicity prime irreducible radical unique-factorization ufd gcd divisibility no-duplicate-factors nodup integer coprime
