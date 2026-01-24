---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Quotient
generated: 2026-01-25T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Quotient

## Overview

The `Quotient/` directory formalizes quotient modules `M ⧸ p` where `p` is a submodule of `M`. Elements of `M` are identified when their difference lies in `p`, creating a new module structure. The directory establishes foundational definitions (quotient construction, quotient map `mkQ`, module structure), lifting and mapping operations (lifting maps through quotients via `liftQ` and `mapQ`, factorization through intermediate quotients), correspondence theorems (order isomorphism between submodules of `M ⧸ p` and submodules of `M` containing `p`), and specialized constructions for pi types (quotient of direct sum equals direct sum of quotients via `quotientPi`).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: quotient equivalence relation (`quotientRel` defining `x ≈ y` iff `x - y ∈ p`), quotient type `M ⧸ p` with quotient map `mk`, module structure (addition, scalar multiplication, zero), linear quotient map `mkQ : M →ₗ[R] M ⧸ p`, and equivalences for equal submodules (`quotEquivOfEq`) |
| Basic.lean | Quotient module theory: scalar restriction equivalences (`restrictScalarsEquiv`), nontriviality and subsingleton characterizations, lifting maps to quotients (`liftQ` for kernel conditions, `liftQSpanSingleton` for span singletons), quotient mapping (`mapQ` between quotients, composition laws, power iteration), factorization (`factor` mapping between quotients of nested submodules), correspondence theorem (`comapMkQRelIso` order isomorphism), and quotient equivalences for isomorphic submodules (`Quotient.equiv`) |
| Card.lean | Cardinality theorem: `card_eq_card_quotient_mul_card` proving `|M| = |S| * |M ⧸ S|` via product-quotient equivalence |
| Pi.lean | Quotients and direct sums: lifting to direct sum of quotients (`piQuotientLift` creating maps from `∀ i, Ms i ⧸ p i`), lifting from quotient of direct sum (`quotientPiLift` creating maps from `(∀ i, Ms i) ⧸ pi p`), and canonical equivalence `quotientPi : ((∀ i, Ms i) ⧸ pi p) ≃ₗ[R] ∀ i, Ms i ⧸ p i` proving quotient of direct sum equals direct sum of quotients |

## Subdirectories

(none)

## Search Tags

quotient-modules quotient-map mkQ liftQ mapQ correspondence-theorem submodule-quotient factor-map direct-sum-quotient pi-quotient cardinality lifting-maps quotient-equivalence restrictScalars nontriviality quotientRel
