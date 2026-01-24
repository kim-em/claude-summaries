---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/ExteriorAlgebra
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# ExteriorAlgebra

## Overview

The `ExteriorAlgebra/` directory formalizes exterior algebras (also known as Grassmann algebras) of modules over commutative rings. The exterior algebra is constructed as a special case of the Clifford algebra with zero quadratic form (`CliffordAlgebra (0 : QuadraticForm R M)`), inheriting the universal property that generators square to zero. The directory establishes the grading structure showing the exterior algebra decomposes as a direct sum of exterior powers, provides the universal property via a lifting construction for alternating maps, and includes functoriality for morphisms between exterior algebras. The implementation covers both the algebraic structure (algebra homomorphisms, injectivity/surjectivity conditions) and the alternating multilinear perspective (extending alternating maps to the full exterior algebra).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core exterior algebra construction: definition as `CliffordAlgebra (0 : QuadraticForm R M)`, canonical injection `ι : M →ₗ[R] ExteriorAlgebra R M` with `ι_sq_zero`, exterior powers `⋀[R]^n M` as range powers, universal property `lift` for maps satisfying squaring-to-zero condition, `ιMulti` for wedge products of vectors (alternating maps to exterior algebra), functoriality via `map` for linear maps between modules, and injectivity/surjectivity characterizations |
| Grading.lean | Grading structure: `gradedAlgebra` instance showing exterior algebra is ℕ-graded by exterior powers `⋀[R]^i M`, graded injection `GradedAlgebra.ι` into direct sum, proof that `ιMulti` images span each graded component and their union spans the entire algebra, compatible with Submodule.nat_power_gradedMonoid structure |
| OfAlternating.lean | Extension from alternating maps: `liftAlternating` constructs linear maps from exterior algebra given alternating maps on each arity (one per exterior power), proves `liftAlternating f (ιMulti R n v) = f n v`, establishes `liftAlternatingEquiv` as linear equivalence between `(∀ i, M [⋀^Fin i]→ₗ[R] N)` and `ExteriorAlgebra R M →ₗ[R] N`, and `lhom_ext` extensionality principle (linear maps agree if they agree on all exterior powers) |

## Subdirectories

(none)

## Search Tags

exterior-algebra grassmann-algebra alternating wedge-product clifford-algebra graded-algebra universal-property multilinear exterior-powers functoriality
