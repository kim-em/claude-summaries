---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/PeriodicPts
generated: 2025-01-24T22:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# PeriodicPts

## Overview

This folder formalizes the theory of periodic points for endomorphisms in Mathlib. A point `x` is periodic under `f : α → α` with period `n` if `f^[n] x = x`. The theory includes core definitions (`IsPeriodicPt`, `periodicPts`, `minimalPeriod`, `periodicOrbit`), algebraic operations on periods (addition, multiplication, gcd, lcm), and connections to group/monoid actions via `MulAction.period`. The formalization supports both general endomorphisms and structured settings (products, Pi types, finite types).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions and basic properties: `IsPeriodicPt f n x` (periodic point predicate), `ptsOfPeriod f n` (set of period-n points), `periodicPts f` (all periodic points), `minimalPeriod f x` (smallest positive period), `periodicOrbit f x` (cycle representation); includes arithmetic on periods (add, sub, mul, gcd, mod), bijectivity of `f` on periodic point sets, orbit membership lemmas, and `MulAction.period`/`AddAction.period` for group actions |
| Lemmas.lean | Additional lemmas building on Defs.lean: characterization of minimal period for prime and prime-power cases, composition formulas for commuting functions (lcm and product of periods), finiteness results (`minimalPeriod_le_card`, factorial periodicity), injectivity characterizations via periodic points, and minimal period formulas for product and Pi types |

## Subdirectories

(none)

## Search Tags

periodic-points minimal-period periodic-orbit isperiodicpt periodicpts iteration fixed-points group-action mulaction-period addaction-period commute composition lcm gcd finite-type orbit cycle dynamical-systems
