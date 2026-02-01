---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/QuasiFinite
generated: 2026-02-01T09:15:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 1
subdirs_count: 0
---

# QuasiFinite

## Overview

This directory contains the theory of quasi-finite algebras in commutative algebra. An R-algebra S is quasi-finite if κ(p) ⊗[R] S is finite-dimensional over the residue field κ(p) for all primes p of R. The formalization differs slightly from the Stacks Project definition by not requiring finite type. The file establishes fundamental properties including stability under base change, composition, localization, and quotients, as well as key theorems relating quasi-finiteness to finite fibers in the prime spectrum.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `Algebra.QuasiFinite` class and `Algebra.QuasiFiniteAt` (quasi-finite at a prime); proves finite fibers property, equivalence with module-finiteness over Artinian rings, stability under base change/composition/localization/quotients, characterization via finite spectrum preimages for finite-type algebras, and applications to polynomial rings showing R[X] is never quasi-finite over R at any prime |

## Subdirectories

(none)

## Search Tags

quasi-finite algebra finite-fiber residue-field base-change localization artinian ring-theory prime-spectrum tensor-product module-finite polynomial algebra-finiteType stacks-project
