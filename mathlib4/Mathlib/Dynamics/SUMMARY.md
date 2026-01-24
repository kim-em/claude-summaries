---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics
generated: 2025-01-24T12:00:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 5
subdirs_count: 6
---

# Dynamics

## Overview

The `Dynamics/` directory formalizes dynamical systems theory in Mathlib, encompassing continuous flows, discrete iterations, ergodic theory, and topological dynamics. It defines flows as continuous monoid actions on topological spaces, provides constructs for studying invariant sets, orbits, omega-limits, and semiconjugacies between flows. The directory includes ergodic theory foundations (measure-preserving maps, conservative dynamics, ergodic theorems), fixed point theorems, periodic point theory, and topological entropy for measuring dynamical complexity.

## Key Files

| File | Purpose |
|------|---------|
| Flow.lean | Defines flows as continuous monoid actions (`Flow τ α`), invariant sets (`IsInvariant`, `IsForwardInvariant`), orbits, forward orbits, flow restriction, semiconjugacies between flows, and time-reversal; includes construction of flows from continuous function iteration |
| Minimal.lean | Defines minimal actions (`MulAction.IsMinimal`, `AddAction.IsMinimal`) where every orbit is dense; proves that pretransitive actions are minimal, and characterizes minimal actions via closed invariant sets |
| Newton.lean | Formalizes Newton-Raphson iteration (`Polynomial.newtonMap`) for root finding; proves fixed points correspond to roots, and establishes existence/uniqueness of nilpotent decomposition for almost-roots (useful for Jordan-Chevalley decomposition) |
| OmegaLimit.lean | Defines omega-limit sets (`omegaLimit`) as asymptotic limit points under flows; provides notation `ω`, `ω⁺`, `ω⁻`; proves properties including closedness, invariance, compactness results, and behavior under set operations |
| Transitive.lean | Defines topologically transitive actions (`MulAction.IsTopologicallyTransitive`) where any two nonempty open sets can be connected by the group action; proves equivalence with dense orbit unions and shows minimal implies transitive |

## Subdirectories

- [x] `BirkhoffSum/` - Birkhoff sums (time averages along orbits) for dynamical systems and ergodic theory
- [x] `Circle/` - Circle dynamics, including rotation number theory for circle homeomorphisms
- [x] `Ergodic/` - Ergodic theory: measure-preserving transformations, ergodic maps, conservative dynamics, and related theorems
- [ ] `FixedPoints/` - Fixed point theorems and related topology for dynamical systems
- [ ] `PeriodicPts/` - Periodic points of dynamical systems, including definitions and key lemmas
- [ ] `TopologicalEntropy/` - Topological entropy theory measuring dynamical complexity via covers, nets, and entourages

## Search Tags

dynamics dynamical-systems flows continuous-monoid-action invariant-sets orbits omega-limit-sets ergodic-theory measure-preserving conservative-dynamics topological-entropy periodic-points fixed-points minimal-actions transitive-actions newton-raphson rotation-number birkhoff-sums circle-dynamics semiconjugacy
