---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics
generated: 2026-01-24T08:00:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 6
---

# Dynamics

## Overview

The `Dynamics/` directory provides a comprehensive formalization of dynamical systems theory spanning both topological and measure-theoretic perspectives. At its foundation, the directory defines flows as continuous monoid actions on topological spaces with detailed theory of invariant sets, orbits, omega-limit sets, and semiconjugacies. The topological dynamics thread includes minimal and transitive actions, fixed point and periodic point theory with full arithmetic on periods, circle dynamics with rotation number theory for degree-one lifts, and topological entropy measuring dynamical complexity via Bowen-Dinaburg's definitions using covers and nets in uniform spaces.

The ergodic theory development provides a complete foundation for statistical mechanics and probability, formalizing measure-preserving transformations, conservative dynamics with Poincare recurrence theorems (both measure-theoretic and topological), and ergodic maps characterized as extreme points of invariant measure sets. The theory proves that invariant functions are a.e. constant under ergodic maps, includes Radon-Nikodym derivative theory for invariant measures, concrete ergodicity results for additive circle maps (multiplication maps and irrational rotations), and extends naturally to group actions showing minimal actions imply ergodicity on compact spaces. The Birkhoff sum framework supports time averages along orbits essential for ergodic theorems, with development in normed spaces including equicontinuity and convergence properties. The directory also includes Newton-Raphson iteration theory with nilpotent decomposition results.

## Key Files

| File | Purpose |
|------|---------|
| Flow.lean | Defines flows as continuous monoid actions (`Flow τ α`), invariant sets (`IsInvariant`, `IsForwardInvariant`), orbits, forward orbits, flow restriction, semiconjugacies between flows, and time-reversal; includes construction of flows from continuous function iteration |
| Minimal.lean | Defines minimal actions (`MulAction.IsMinimal`, `AddAction.IsMinimal`) where every orbit is dense; proves that pretransitive actions are minimal, and characterizes minimal actions via closed invariant sets |
| Newton.lean | Formalizes Newton-Raphson iteration (`Polynomial.newtonMap`) for root finding; proves fixed points correspond to roots, and establishes existence/uniqueness of nilpotent decomposition for almost-roots (useful for Jordan-Chevalley decomposition) |
| OmegaLimit.lean | Defines omega-limit sets (`omegaLimit`) as asymptotic limit points under flows; provides notation `ω`, `ω⁺`, `ω⁻`; proves properties including closedness, invariance, compactness results, and behavior under set operations |
| Transitive.lean | Defines topologically transitive actions (`MulAction.IsTopologicallyTransitive`) where any two nonempty open sets can be connected by the group action; proves equivalence with dense orbit unions and shows minimal implies transitive |

## Subdirectories

- [x] `BirkhoffSum/` - Birkhoff sums `∑_{k<n} g(f^k(x))` and averages along orbits; includes basic identities, almost-invariance properties, normed space theory with equicontinuity for Lipschitz maps, and quasi-measure-preserving results for a.e. equality
- [x] `Circle/` - Circle dynamics via degree-one lifts (monotone maps `f: ℝ → ℝ` with `f(x+1) = f(x)+1`); translation number theory with τ(f) = lim (f^n(x)-x)/n, semiconjugacy results, orbit equivalence, and connections to Poincare's rotation number for circle homeomorphisms
- [x] `Ergodic/` - Complete ergodic theory foundation: measure-preserving maps, conservative dynamics with Poincare recurrence, ergodic/quasi-ergodic definitions, zero-one laws, invariant functions are a.e. constant, ergodic measures as extreme points, Radon-Nikodym derivative invariance, concrete examples on additive circle (multiplication and irrational rotation), and group action ergodicity linking minimal actions to ergodicity on compact spaces
- [x] `FixedPoints/` - Fixed point foundations with `IsFixedPt f x` predicate and `fixedPoints f` set; algebraic properties for composition/iteration/semiconjugacy/permutations, topological results (closedness in T2, convergence of iterates), and Prufer subgroup invariance for circle dynamics
- [x] `PeriodicPts/` - Comprehensive periodic point theory: `IsPeriodicPt f n x` predicate, `periodicPts f` and `ptsOfPeriod f n` sets, `minimalPeriod f x`, `periodicOrbit f x` cycles, arithmetic on periods (add/mul/gcd/lcm), characterizations for primes and prime powers, composition formulas for commuting functions, finiteness results, and minimal period formulas for products and Pi types
- [x] `TopologicalEntropy/` - Topological entropy via Bowen-Dinaburg definitions in uniform spaces: dynamical entourages tracking orbit proximity, cover-based entropy (minimal dynamical covers), net-based entropy (maximal distinguishable orbit sets), equivalence proofs, entropy under semiconjugacies, and functorial properties (monotonicity, closure, union formulas)

## Search Tags

dynamics dynamical-systems flows continuous-monoid-action invariant-sets orbits omega-limit-sets ergodic-theory measure-preserving conservative-dynamics topological-entropy periodic-points fixed-points minimal-actions transitive-actions newton-raphson rotation-number birkhoff-sums circle-dynamics semiconjugacy
