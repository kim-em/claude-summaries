---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/Ergodic
generated: 2026-01-24T05:30:20Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 1
---

# Ergodic

## Overview

The `Ergodic/` directory formalizes the mathematical foundations of ergodic theory in Mathlib. It defines measure-preserving transformations, conservative dynamical systems, and ergodic maps, along with their key properties. The theory includes Poincare recurrence theorems (both measure-theoretic and topological), quasi-ergodicity, characterizations of ergodic measures as extreme points of invariant measure sets, and concrete examples of ergodic maps on the additive circle. The directory also establishes that invariant functions under ergodic maps are a.e. constant and develops the Radon-Nikodym derivative theory for invariant measures.

The `Action/` subdirectory extends these concepts to group and monoid actions, defining `ErgodicSMul` and `ErgodicVAdd` typeclasses. It proves that regular group actions are ergodic with respect to invariant measures, and establishes connections between minimal actions and ergodicity—showing that minimal group actions on compact spaces imply ergodicity with respect to Haar measure.

## Key Files

| File | Purpose |
|------|---------|
| MeasurePreserving.lean | Defines `MeasurePreserving` predicate for maps with `map f mu = nu`; provides composition, iteration, restriction, and conjugation lemmas; proves pigeonhole-based results showing points return under iteration |
| Ergodic.lean | Defines `PreErgodic`, `Ergodic`, and `QuasiErgodic` structures for maps where invariant sets are a.e. trivial; proves zero-one laws on probability spaces; shows ergodic implies quasi-ergodic; includes conjugacy invariance |
| Conservative.lean | Defines `Conservative` dynamical systems where points return to positive-measure sets; proves measure-theoretic and topological Poincare recurrence theorems; shows iteration of conservative maps is conservative |
| Function.lean | Proves that a.e. invariant functions under (quasi)ergodic maps are a.e. constant; handles both measurable and a.e. strongly measurable functions; includes `AEEqFun` quotient space versions |
| AddCircle.lean | Proves ergodicity of `n`-fold multiplication maps on `AddCircle T` for `|n| > 1`; uses Lebesgue density theorem and rational rotation invariance arguments |
| AddCircleAdd.lean | Proves irrational rotations on `AddCircle` are ergodic iff the rotation has infinite order (i.e., the angle/period is irrational) |
| Extreme.lean | Characterizes ergodic measures as extreme points of the convex set of invariant measures with fixed total mass; proves uniqueness of ergodic measures up to scaling when one is absolutely continuous w.r.t. the other |
| RadonNikodym.lean | Proves singular parts, absolutely continuous parts, and Radon-Nikodym derivatives of invariant measures are themselves invariant under measure-preserving maps |

## Subdirectories

- [x] `Action/` - Ergodicity for group actions, including minimal actions and regular actions

## Search Tags

ergodic-theory measure-preserving ergodic quasi-ergodic conservative poincare-recurrence invariant-measure additive-circle irrational-rotation radon-nikodym extreme-points probability-measure zero-one-law dynamical-systems measure-theory
