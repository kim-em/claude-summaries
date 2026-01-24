---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/GeneralLinearGroup
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# GeneralLinearGroup

## Overview

The `GeneralLinearGroup/` subdirectory contains the theory of general linear groups GL(R,M), defined as the group of invertible linear maps from a module M to itself. This directory establishes the foundational correspondence between invertible linear maps (units in the endomorphism monoid) and linear equivalences, provides functorial behavior under module isomorphisms, and proves that algebra automorphisms of endomorphism algebras are always inner automorphisms (conjugation by GL elements). The implementation covers both the basic definition and structure, as well as deep structural theorems about endomorphism algebras.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | General linear group definition: `GeneralLinearGroup R M` as units of `M →ₗ[R] M`, bidirectional conversion with linear equivalences (`toLinearEquiv`, `ofLinearEquiv`), multiplicative equivalence `generalLinearEquiv : GeneralLinearGroup R M ≃* M ≃ₗ[R] M`, and functoriality via `congrLinearEquiv` (isomorphism of GL groups induced by semilinear module equivalences) |
| AlgEquiv.lean | Inner automorphism characterization: proof that algebra equivalences `End K V ≃ₐ[K] End K W` for projective modules are always conjugation by linear equivalences (`AlgEquiv.eq_linearEquivConjAlgEquiv`), surjectivity of conjugation map (`LinearEquiv.conjAlgEquiv_surjective`), and equivalence with `MulSemiringAction.toAlgEquiv` surjectivity for V=W case |

## Subdirectories

(No subdirectories)

## Search Tags

general-linear-group linear-equivalence invertible-linear-maps endomorphisms algebra-automorphisms inner-automorphisms conjugation projective-modules units functoriality semilinear-maps
