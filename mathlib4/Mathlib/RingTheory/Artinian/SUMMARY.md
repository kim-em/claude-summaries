---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Artinian
generated: 2026-01-26T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Artinian

## Overview

This folder contains the formalization of Artinian modules and rings in Lean 4. A module is Artinian if every decreasing chain of submodules stabilizes (descending chain condition), equivalently if the strict submodule relation is well-founded. The theory includes basic properties, closure under quotients and direct sums, the Fitting decomposition for endomorphisms, semisimplicity characterizations via the Jacobson radical, and ring-specific results including the finite spectrum theorem and structure theorems for reduced Artinian rings.

## Key Files

| File | Purpose |
|------|---------|
| Module.lean | Core definitions and theory of Artinian modules: `IsArtinian` predicate, stability of decreasing chains, induction principles, injective endomorphisms are surjective, Fitting decomposition, semisimplicity iff Jacobson radical is zero, finite spectrum for Artinian rings, structure theorem (reduced commutative Artinian ring ≃ product of fields) |
| Ring.lean | Additional Artinian ring theory: localization surjectivity, nilpotency of Jacobson radical, equivalence of radical and Jacobson in Artinian rings, reduced local Artinian rings are fields |
| Algebra.lean | Artinian ring theory for algebras: integral elements over Artinian rings are units iff non-zero-divisors, characterization of unit submonoid in integral extensions |
| Instances.lean | Decomposition monoid instances: reduced Artinian rings and polynomial rings over them are decomposition monoids, strong rank condition for Artinian modules |

## Subdirectories

(none)

## Search Tags

Artinian descending-chain-condition DCC well-founded submodule Fitting-decomposition injective-endomorphism surjective Jacobson-radical semisimple spectrum maximal-ideal prime-ideal finite-spectrum reduced-ring product-of-fields localization nilpotent integral-element zero-divisor unit decomposition-monoid strong-rank-condition Hopkins-Levitzki Atiyah-Macdonald
