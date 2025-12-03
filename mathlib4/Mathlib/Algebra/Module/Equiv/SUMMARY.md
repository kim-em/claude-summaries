---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module/Equiv
generated: 2025-12-01T08:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Equiv

## Overview

The `Equiv/` directory defines linear equivalences (invertible linear maps) between modules. It provides the core `LinearEquiv` structure (notation `M ≃ₗ[R] M₂`) which bundles an invertible linear map with explicit inverse and bidirectional linearity proofs. The directory includes extensive theory for semilinear equivalences (with respect to ring homomorphisms `σ : R →+* S`), equivalence class abstractions, operations on equivalences (composition, symmetry, restriction of scalars), special constructors (from units, field elements, additive equivalences), and the automorphism group structure on `M ≃ₗ[R] M` with distributive multiplicative action.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `LinearEquiv σ M M₂` structure extending `LinearMap` and `AddEquiv` with inverse, `SemilinearEquivClass` typeclass, basic operations (refl, symm, trans), coercion lemmas, and equivalence properties |
| Basic.lean | Extended theory: scalar restriction (`restrictScalars`), automorphism group structure with multiplication as composition, distributive action on modules, constructors from subsingletons/units/field elements, conversions from additive equivalences, arrow congruence, conjugation of endomorphisms, function congruence for dependent products |
| Opposite.lean | Linear equivalences on opposite modules: `MulOpposite.opLinearEquiv : M ≃ₗ[R] Mᵐᵒᵖ` preserving scalar multiplication, ring operator extension lemma |

## Subdirectories

None.

## Search Tags

linear-equivalence linear-isomorphism module-isomorphism invertible-linear-map semilinear-equivalence automorphism-group scalar-restriction additive-equivalence opposite-module conjugation arrow-congruence
