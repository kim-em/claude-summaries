---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/Algebra
generated: 2026-01-24T18:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Algebra

## Overview

The `Algebra/` directory provides the algebraic infrastructure for smooth manifolds, particularly Lie groups and related structures. It defines `C^n` monoids (`ContMDiffMul`), Lie groups (`LieGroup`), and smooth rings (`ContMDiffRing`), establishing that manifolds with smooth group/ring operations inherit the corresponding algebraic structures. The library also shows that spaces of smooth functions `C^n⟮I, M; I', G⟯` inherit algebraic structures (group, ring, module, algebra) from their target spaces, and defines left-invariant derivations as an approach to Lie algebras of Lie groups.

## Key Files

| File | Purpose |
|------|---------|
| Monoid.lean | Defines `ContMDiffMul` and `ContMDiffAdd` typeclasses for `C^n` monoids/semigroups; proves smoothness of products, powers, and finite products; defines `ContMDiffMonoidMorphism` for smooth monoid homomorphisms; provides `smoothLeftMul` (`𝑳`) and `smoothRightMul` (`𝑹`) notation |
| LieGroup.lean | Defines `LieGroup` and `LieAddGroup` typeclasses (group + manifold with smooth multiplication and inversion); proves smoothness of pointwise inv/div; defines `ContMDiffInv₀` for smoothness of inversion away from zero (applies to complete normed fields) |
| Structures.lean | Defines `ContMDiffRing` typeclass for smooth semirings; shows `ContMDiffRing` implies `ContMDiffMul` and `LieAddGroup`; proves any nontrivially normed field is a `ContMDiffRing` |
| SmoothFunctions.lean | Equips `C^n⟮I, N; I', G⟯` with algebraic instances: Mul, Monoid, Group, Semiring, Ring, Module, Algebra; defines `coeFnMonoidHom`, `coeFnRingHom`, `coeFnAlgHom`; provides restriction homomorphisms for open subsets |
| LeftInvariantDerivation.lean | Defines `LeftInvariantDerivation I G` (global derivations invariant under pullback by left multiplication); proves this forms a Lie algebra; provides `evalAt` for point evaluation; relates to the tangent space at identity |

## Subdirectories

(none)

## Search Tags

lie-group lie-algebra contmdiffmul contmdiffadd contmdiffring smooth-monoid smooth-group smooth-ring left-invariant-derivation smooth-functions-algebra pointwise-multiplication lie-add-group contmdifinv0 smooth-left-mul smooth-right-mul
