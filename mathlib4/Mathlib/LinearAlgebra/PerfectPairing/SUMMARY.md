---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/PerfectPairing
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# PerfectPairing

## Overview

The `PerfectPairing/` directory formalizes perfect pairings between modules, which are bilinear maps `M × N → R` that induce bijections `M ≃ Dual R N` and `N ≃ Dual R M`, establishing reflexivity of both modules. The theory includes the core definition (`IsPerfPair`), connections to linear equivalences with dual spaces, perfect complementarity of submodules, restriction to submodules, and scalar restriction from rings to subrings or fields to subfields. Matrix.lean provides deprecated legacy support for viewing invertible matrices as perfect pairings via dot products.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core perfect pairing theory: `IsPerfPair` typeclass (bijectivity in both arguments), equivalence with dual spaces (`toPerfPair : M ≃ₗ[R] Dual R N`), reflexivity proofs, perfect complementarity (`IsPerfectCompl` for dual annihilators), and connections between linear equivalences `N ≃ₗ[R] Dual R M` and perfect pairings |
| Restrict.lean | Restriction operations: restriction to submodules (`IsPerfPair.restrict` for perfectly complementary submodules), restriction of scalars to subrings (`IsPerfPair.restrictScalars`), and field-specific restriction (`IsPerfPair.restrictScalars_of_field` for simultaneously restricting domains and coefficients from field extensions) |
| Matrix.lean | Deprecated matrix connection: `Matrix.toPerfectPairing` views invertible matrices as perfect pairings via `toLinearEquiv'` composed with `dotProductEquiv` (deprecated since 2025-08-16 with no replacement) |

## Subdirectories

*(No subdirectories)*

## Search Tags

perfect-pairing bilinear-forms dual-spaces reflexive-modules linear-equivalences submodule-restriction scalar-restriction field-extensions annihilators complementary-submodules duality matrix-pairing
