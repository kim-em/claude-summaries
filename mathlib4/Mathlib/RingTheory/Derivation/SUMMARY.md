---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Derivation
generated: 2026-01-26T19:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Derivation

## Overview

The `Derivation/` directory contains the theory of derivations on algebras and rings. A derivation `D : Derivation R A M` is an R-linear map from an R-algebra A to an A-module M satisfying the Leibniz rule `D(ab) = a·Db + b·Da`. This directory provides the core definition, module and Lie algebra structures on derivations, typeclass support for differential rings, polynomial applications, and the correspondence between derivations into square-zero ideals and algebra lifts.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Derivation R A M` structure; Leibniz rule; addition, scalar multiplication, module structure; composition with linear maps (`llcomp`); pushforward through linear equivalences; restriction and extension of scalars; lifting derivations via algebra homomorphisms; polynomial evaluation rules (`map_aeval`); extensionality principles |
| Lie.lean | Lie algebra structure on derivations; commutator `⁅D1, D2⁆ = D1 ∘ D2 - D2 ∘ D1` is a derivation; `Derivation R A A` forms a Lie ring and Lie algebra over R |
| DifferentialRing.lean | Typeclass `Differential R` for rings with a canonical derivation; postfix notation `x′` for derivatives; `DifferentialAlgebra` class ensuring derivation commutes with `algebraMap`; `ContainConstants` class for when constants are exactly the kernel of the derivation |
| MapCoeffs.lean | Coefficient-wise derivation on polynomials; `mapCoeffs : Derivation R A[X] (PolynomialModule A M)` applies derivation to each coefficient; key formula `D(p(x)) = (D.mapCoeffs p)(x) + D(x) · p'(x)` relating evaluation, coefficient derivatives, and formal derivative; specialization to differential rings with `x′` notation |
| ToSquareZero.lean | Derivations into square-zero ideals; `derivationToSquareZeroEquivLift`: R-derivations `A → I` (where I² = 0) correspond bijectively to lifts `A →ₐ[R] B` of the quotient map `A →ₐ[R] B/I`; used in deformation theory and infinitesimal lifting problems |

## Subdirectories

None.

## Search Tags

derivation Leibniz-rule differential-ring Lie-algebra commutator polynomial coefficient-derivative square-zero-ideal lifting-problem deformation-theory R-linear-map module-structure algebraMap differential-algebra constants kernel evaluation aeval formal-derivative tower-of-algebras scalar-restriction
