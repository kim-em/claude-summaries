---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/NumberField/CanonicalEmbedding
generated: 2026-01-25T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# CanonicalEmbedding

## Overview

The canonical embedding of a number field `K` is the injective ring homomorphism `K →+* ((K →+* ℂ) → ℂ)` that maps each element `x ∈ K` to the vector of its images under all complex embeddings. For computational purposes, this can be reformulated as the mixed embedding into `ℝ^r₁ × ℂ^r₂` where `(r₁, r₂)` is the signature of `K`. This directory provides the full theory of canonical and mixed embeddings, including applications to lattice theory (integer lattices and fractional ideal lattices), convex geometry (Minkowski's Convex Body Theorem), unit theory (fundamental domains and Dirichlet's Unit Theorem), and polar coordinate change of variables for volume computations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `canonicalEmbedding` (into `ℂ^n`), `mixedEmbedding` (into `ℝ^r₁ × ℂ^r₂`), lattice structures for ring of integers and fractional ideals, injectivity proofs, norm computations, and finiteness results for integer lattice intersections with balls |
| ConvexBody.lean | Convex bodies in mixed space for applying Minkowski's Convex Body Theorem: `convexBodyLT` (points with `‖x w‖ < f w` for all infinite places), `convexBodySum` (sum of norms bounded), volume computations, and existence theorems for nonzero elements in fractional ideals satisfying norm bounds |
| FundamentalCone.lean | Action of units `(𝓞 K)ˣ` on mixed space via multiplication, fundamental cone as fundamental domain for unit action modulo torsion, `logMap` and connection to Dirichlet Unit Theorem, ideal sets and their equivalence with principal ideals of given norm |
| NormLeOne.lean | Subset `normLeOne` of the fundamental cone consisting of elements with `mixedEmbedding.norm x ≤ 1`, proof of boundedness, volume computation via polar coordinates and change of variables (`expMapBasis` map), frontier has measure zero, connection to regulator and class number formula |
| PolarCoord.lean | Polar coordinate changes of variables: `polarCoord` (into `ℝ^r₁ × (ℝ × ℝ)^r₂`) and `polarSpaceCoord` (into `ℝ^(r₁+r₂) × ℝ^r₂`), integration formulas for norm-stable sets at complex or all places, volume computation techniques for symmetric subsets of mixed space |

## Subdirectories

None

## Search Tags

canonical-embedding mixed-embedding number-field complex-embeddings infinite-places signature lattice integer-lattice fractional-ideal-lattice minkowski convex-body units fundamental-cone fundamental-domain dirichlet-unit-theorem regulator polar-coordinates volume measure-theory class-number norm-bound existence-theorem
