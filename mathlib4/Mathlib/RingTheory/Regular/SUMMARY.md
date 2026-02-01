---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Regular
generated: 2026-02-01T09:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 5
subdirs_count: 0
---

# Regular

## Overview

The `Regular/` directory formalizes the theory of regular elements and regular sequences in commutative algebra, fundamental concepts for understanding singularities and homological properties of rings and modules. A regular element is a non-zero-divisor on a module (IsSMulRegular), and a regular sequence is an ordered list of elements where each is regular on the quotient by previous elements. The directory includes categorical formulations via short exact complexes, depth theory connecting regularity to homological dimension, stability of regularity under flat base change and localization, and permutation results for regular sequences under Jacobson ideal conditions.

## Key Files

| File | Purpose |
|------|---------|
| IsSMulRegular.lean | Core theory of regular elements (non-zero-divisors) on modules; equivalences with kernel conditions, quotient characterizations, exact sequence lifting, tensor product preservation under flatness, associated primes characterization |
| RegularSequence.lean | Regular and weakly regular sequences on modules; inductive characterizations via quotients, permutation stability under Jacobson/local ring conditions, relationship to Artinian modules, tensor product behavior, depth prerequisites |
| Category.lean | Categorical constructions for IsSMulRegular via short exact complexes; smulShortComplex construction M → M → M⧸xM with exactness properties |
| Depth.lean | Depth theory for modules; relationship between module homomorphisms being subsingleton and existence of regular elements in annihilators; foundational results for depth computations |
| Flat.lean | Stability of (weakly) regular sequences under flat base change; localization and faithfully flat behavior; proves regular sequences lift to localizations and tensor products with flat algebras |

## Subdirectories

(none)

## Search Tags

regular-element regular-sequence weakly-regular depth non-zero-divisor IsSMulRegular module commutative-algebra homological-algebra short-exact-complex flat-base-change localization associated-primes annihilator Jacobson-ideal tensor-product Artinian-module Noetherian Nakayama quotient-module categorical-homology faithfully-flat permutation-stability maximal-ideal local-ring
