---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/DirichletCharacter
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# DirichletCharacter

## Overview

The `DirichletCharacter/` directory contains the theory of Dirichlet characters, which are multiplicative characters from `ZMod n` to a commutative monoid with zero that send non-units to 0. The directory provides the core definitions (including conductor and primitive characters), analytic bounds on character values, Gauss sum theory for primitive characters, and orthogonality relations. These tools are foundational for analytic number theory, particularly the study of L-series and Dirichlet's theorem on primes in arithmetic progressions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `DirichletCharacter`, level changing via `changeLevel`, conductor and primitive characters, even/odd characters, factorization through divisors |
| Bounds.lean | Norm bounds for Dirichlet characters with values in normed fields: `‖χ a‖ = 1` for units, `‖χ a‖ ≤ 1` in general |
| GaussSum.lean | Gauss sums for Dirichlet characters: vanishing when χ is primitive but the additive character is not, functional equation for `gaussSum χ (e.mulShift a)` |
| Orthogonality.lean | Orthogonality relations: sum over all characters vanishes when `a ≠ b` and equals `n.totient` when `a = b`, requires enough roots of unity |

## Subdirectories

*(No subdirectories)*

## Search Tags

dirichlet-character multiplicative-character conductor primitive-character change-level gauss-sum orthogonality roots-of-unity even-odd-character normed-field analytic-number-theory
