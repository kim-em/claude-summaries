---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Etale
generated: 2026-01-26T20:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# Etale

## Overview

The `Etale/` directory formalizes étale morphisms and algebras in commutative algebra. An R-algebra A is formally étale if both the Kähler differential module Ω[A⁄R] and the first cotangent cohomology H¹(L_{A/R}) vanish, which is equivalent to the standard infinitesimal lifting property for square-zero extensions. An algebra is étale if it is formally étale and of finite presentation. This directory provides the foundational theory, characterizations over fields (as finite products of separable extensions), relationships with Kähler differentials, étale loci, product structures, quasi-finite properties, and standard étale presentations via polynomial quotients.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of formally étale and étale algebras; equivalence with infinitesimal lifting property; stability under isomorphisms, composition, base change, and localization |
| Field.lean | Characterization of formally étale field extensions as separable extensions; étale algebras over fields as finite products of finite separable field extensions |
| Kaehler.lean | Relationship between étale algebras and Kähler differentials; canonical isomorphisms T ⊗[S] Ω[S⁄R] ≃ T ⊗[R] for formally étale S→T; base change properties for cotangent complexes |
| Locus.lean | Étale locus (set of primes where localization is formally étale); openness in finite type case; characterization via support of differential modules |
| Pi.lean | Formal étaleness of finite products; characterization that Π i, A i is formally étale iff each A i is formally étale |
| QuasiFinite.lean | Étale local structure of finite maps; construction of étale neighborhoods splitting fibers; existence of étale R-algebras with prescribed fiber decompositions |
| StandardEtale.lean | Standard étale algebras as R[X][Y]/⟨f, Yg-1⟩ where f is monic and f' invertible mod (f,g); equivalences with (R[X]/f)[1/g] and R[X][1/g]/f; universal property via roots with invertible image |

## Subdirectories

(none)

## Search Tags

etale formally-etale ring-theory commutative-algebra morphism unramified smooth separable field-extension Kaehler-differential cotangent-complex infinitesimal-lifting square-zero finite-presentation localization base-change fiber quasi-finite standard-etale polynomial-quotient residue-field prime-spectrum locus
