---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Unramified
generated: 2026-02-01T22:00:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 6
subdirs_count: 0
---

# Unramified

## Overview

The `Unramified/` directory contains the theory of formally unramified and unramified algebras in commutative ring theory. An R-algebra A is formally unramified if its Kähler differentials Ω[A/R] are trivial, which is equivalent to the unique lifting property for square-zero extensions. An algebra is unramified if it is formally unramified and of finite type. This includes characterizations in special settings (fields, local rings), structural theorems (finite generation of free unramified algebras), stability results (composition, base change, localization), and geometric aspects (unramified locus as open subset of the spectrum).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and properties of formally unramified and unramified algebras; defines FormallyUnramified class via triviality of Kähler differentials; proves equivalence with unique lifting property for square-zero extensions; stability under isomorphisms, composition, quotients, base change, and localization |
| Field.lean | Unramified algebras over fields; proves field extensions are unramified iff separable; shows unramified algebras over algebraically closed fields are isomorphic to the field; proves unramified algebras over fields are reduced; establishes bijective algebraMap for local unramified algebras over algebraically closed fields |
| Finite.lean | Various finiteness and structural results for unramified algebras; proves finite-type unramified algebras satisfy tensor product characterization with annihilating idempotent; shows unramified free algebras are finitely generated (Iversen I.2.8); proves R-flat implies S-flat for unramified S over R; constructs S-linear section of tensor product map |
| LocalRing.lean | Unramified algebras over local rings; characterizes unramified local algebras via residue field separability and maximal ideal equality (m_R·S = m_S); proves unramified locus criterion for prime ideals (κ(q)/κ(p) separable and pS_q = qS_q); shows residue field extensions of unramified algebras are finite and separable |
| Locus.lean | Geometric notion of unramified locus; defines IsUnramifiedAt for prime ideals and unramifiedLocus as set of unramified primes in Spec(A); characterizes locus as complement of support of Kähler differentials; proves basicOpen subsets contained in locus iff localization is unramified; shows unramified locus is open for finite-type algebras |
| Pi.lean | Unramified property for finite products; proves finite product Π i, A i is formally unramified over R iff each A i is formally unramified over R; uses idempotent elements to reduce to individual factors |

## Subdirectories

(none)

## Search Tags

unramified formally-unramified Kaehler-differential separable field-extension local-ring residue-field maximal-ideal tensor-product finite-type flat free algebra localization base-change composition spectrum unramified-locus
