---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/PolynomialLaw
generated: 2026-02-01T12:00:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 1
subdirs_count: 0
---

# PolynomialLaw

## Overview

This folder formalizes polynomial laws on modules, following Roby's 1963 theory. A polynomial law `f : M →ₚₗ[R] N` between R-modules assigns functorial maps `S ⊗[R] M → S ⊗[R] N` for every R-algebra S. The implementation handles universe polymorphism by lifting tensor products to polynomial rings in the base universe and using direct limits. Polynomial laws form an R-module under pointwise operations, and composition is defined. The "ground" function extracts the underlying `M → N` map.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of polynomial laws: defines `PolynomialLaw` structure with `toFun'` and `isCompat'` fields; module structure on polynomial laws (addition, scalar multiplication, negation); identity and composition; `ground` function mapping polynomial laws to functions; universe-polymorphic extension `toFun` using lifts through multivariate polynomial rings; proofs that functoriality extends across universes |

## Subdirectories

(none)

## Search Tags

polynomial-law polynomial-map module-functor tensor-product R-algebra functorial natural-transformation universe-polymorphism Roby multivariate-polynomial lift ground composition
