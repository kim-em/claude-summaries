---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Matrix/GeneralLinearGroup
generated: 2026-01-25T22:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# GeneralLinearGroup

## Overview

The `GeneralLinearGroup/` subdirectory contains the formalization of the general linear group GL(n, R), consisting of all invertible n×n matrices over a ring R. It defines GL(n, R) as the units of the matrix ring, establishes connections to linear maps via `toLin`, and provides constructors for building GL elements from matrices with invertible determinants. The directory includes specialized theory for GL(2), covering parabolic/hyperbolic/elliptic classifications of 2×2 matrices based on discriminant, fixed-point polynomials for Möbius transformations, and cardinality formulas for GL over finite fields. The implementation connects matrix invertibility to determinant units, scalar centers, and ring homomorphism functoriality.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core GL definitions: `GeneralLinearGroup n R` as units of matrix ring, determinant homomorphism `det : GL n R →* Rˣ`, equivalences `toLin` and `toLin'` to linear map groups, constructors `mk'`/`mk''`/`mkOfDetNeZero` from matrices with unit determinants, extensionality, coercion lemmas, ring homomorphism functoriality via `map`, Kronecker products of GL elements, embeddings `SpecialLinearGroup → GL → GLPos` |
| Basic.lean | Basic GL lemmas: characterization of center as scalar matrices (`mem_center_iff_val_eq_scalar`), proof that center equals image of units under scalar embedding, example constructions like `planeConformalMatrix` for complex-number-inspired 2×2 matrices |
| Card.lean | Cardinality of GL over finite fields: counts linearly independent vectors (`card_linearIndependent`), establishes equivalence between GL(n, 𝔽) and n linearly independent vectors (`equiv_GL_linearindependent`), proves `card_GL_field` formula ∏ᵢ (qⁿ - qⁱ) for GL over field with q elements |
| FinTwo.lean | Theory of GL(2): parabolic/hyperbolic/elliptic classification via discriminant (parabolic: non-scalar with discr=0, hyperbolic: discr>0, elliptic: discr<0), characterization of parabolic matrices as scalar + nonzero nilpotent, fixed-point polynomial for Möbius transformations, `upperRightHom : AddChar R (GL (Fin 2) R)` sending x to [1, x; 0, 1], conjugation invariance of discriminant and classifications |

## Subdirectories

(none)

## Search Tags

general-linear-group GL invertible-matrices units determinant matrix-group special-linear-group center scalar-matrices toLin matrix-linear-map-equivalence ring-homomorphism kronecker-product parabolic hyperbolic elliptic discriminant GL2 finite-fields cardinality linearly-independent Moebius-transformation fixed-point-polynomial nilpotent upper-triangular GLPos positive-determinant
