---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Extension
generated: 2026-01-26T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 2
---

# Extension

## Overview

The `Extension/` directory provides a complete framework for formalizing algebra extensions, generators, presentations, and the naive cotangent complex in algebraic geometry. At the foundation are two key structures: `Algebra.Extension` (surjective R-algebra homomorphisms P → S) and `Algebra.Generators` (families of generators with polynomial maps R[X] → S). Building on these, the `Presentation/` subdirectory develops the theory of presentations (generators plus relations) and submersive presentations (characterized by invertible Jacobians)—the algebraic foundation for smooth morphisms. The `Cotangent/` subdirectory provides the naive cotangent complex construction for presentations, yielding exact sequences `I/I² → ⨁ᵢ S dxᵢ → Ω[S/R] → 0`, with complete homology theory (H¹ independent of presentation choice), base change and localization formulas, and computational tools for verifying submersivity via Jacobian calculations. This provides the essential algebraic machinery for studying differential properties of algebra homomorphisms in the style of modern algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `Algebra.Extension` structure for extensions P → S with surjection; includes constructions (from surjective maps, trivial extension, localization, base change, infinitesimal extension); homomorphisms between extensions; cotangent space as type synonym for I/I²; cotangent module structure over S and linear maps between cotangent spaces |
| Generators.lean | Defines `Algebra.Generators` structure for families of generators (variables, values, section of R[X] → S); constructions from surjective maps, sets, algebra homomorphisms; composition, base change, extension of scalars, reindexing; homomorphisms between generators; kernel theory including decomposition for composition of generators; relationship to finite type algebras |

## Subdirectories

- [x] `Cotangent/` - Naive cotangent complex theory for algebra presentations: cotangent space construction (I/I² → ⨁ S dxᵢ → Ω[S/R]), exactness results, first homology H¹(L_{S/R}) independent of presentation, base change and localization behavior, Jacobian-based criteria for submersivity
- [x] `Presentation/` - Presentations of algebras (generators plus relations spanning the kernel): presentation dimension, submersive presentations (finite with invertible Jacobian), Jacobi matrix and differential constructions, descent to coefficient subrings for removing Noetherian hypotheses

## Search Tags

algebra-extension generators presentation polynomial-ring multivariate-polynomial surjection section cotangent-space cotangent-complex conormal-space naive-cotangent-complex H1-cotangent first-homology kaehler-differentials infinitesimal-extension base-change localization composition kernel ideal finite-type finite-presentation scalar-tower homomorphism reindexing submersive jacobian jacobi-matrix differential smooth-algebra standard-smooth exact-sequence tensor-product coefficients subalgebra descent noetherian dimension pderiv determinant basis homotopy
