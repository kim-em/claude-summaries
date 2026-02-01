---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Jacobson
generated: 2026-02-01T22:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 6
subdirs_count: 0
---

# Jacobson

## Overview

The `Jacobson/` directory provides a comprehensive formalization of Jacobson radical theory for rings and modules. This includes the Jacobson radical of ideals (intersection of all maximal ideals containing the ideal), the Jacobson radical of modules (intersection of maximal submodules), Jacobson rings (where every radical ideal equals its Jacobson radical), and semiprimary rings (nilpotent Jacobson radical with semisimple quotient). The theory connects these concepts to localization, polynomial rings, and multivariate polynomials, proving key results like preservation of the Jacobson property under quotients, localizations, and polynomial extensions.

## Key Files

| File | Purpose |
|------|---------|
| Radical.lean | Defines `Module.jacobson` (intersection of maximal submodules) and `Ring.jacobson` (Jacobson radical as two-sided ideal); proves functoriality under linear maps, Nakayama's lemma for noncommutative rings, and establishes `Ring.jacobson R • N < N` for finitely generated nonzero `N` |
| Ideal.lean | Defines `Ideal.jacobson I` (intersection of maximal ideals containing `I`) and `Ideal.IsLocal`; provides characterization `mem_jacobson_iff` and proves radical-Jacobson relationships; extends to `TwoSidedIdeal.jacobson` for non-commutative rings |
| Ring.lean | Defines the `IsJacobsonRing` class (radical ideals equal their Jacobson radical); proves equivalence with prime ideal and infimum-of-maximals characterizations; shows Jacobson property preserved under quotients, integral extensions, and localizations; proves `R[X]` is Jacobson iff `R` is; includes Nullstellensatz and Zariski's lemma applications |
| Polynomial.lean | Shows `jacobson (⊥ : Ideal R[X]) ≤ sInf (map C '' maximals)` and proves `jacobson ⊥ = ⊥` for polynomial rings over rings with trivial Jacobson radical |
| Artinian.lean | Connects Artinian rings and Jacobson rings: proves `Module.Finite R A ↔ IsArtinianRing A` for finite type algebras over Artinian rings; shows finite type algebras over Jacobson rings that are Artinian are module-finite |
| Semiprimary.lean | Defines `IsSemiprimaryRing` (nilpotent Jacobson radical with semisimple quotient); proves `IsSemisimpleModule.jacobson_eq_bot` and that semisimple rings have trivial Jacobson radical; shows semisimple commutative rings are reduced |

## Subdirectories

(none)

## Search Tags

Jacobson-radical Jacobson-ring radical-ideal maximal-ideal prime-ideal intersection semiprimary semisimple Nakayama-lemma localization polynomial-ring multivariate-polynomial integral-extension quotient-ring two-sided-ideal module-radical Nullstellensatz Zariski-lemma Artinian finite-type finite-module
