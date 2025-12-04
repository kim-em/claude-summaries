---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/ProjectiveSpectrum
generated: 2025-12-04T13:09:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# ProjectiveSpectrum

## Overview

The `ProjectiveSpectrum/` directory provides the complete formalization of the projective spectrum construction Proj for graded rings, which is the projective analogue of the Spec functor. It defines the topological space of relevant homogeneous prime ideals, constructs the structure sheaf of locally expressible fractions of the same degree, proves that Proj is a scheme via an affine cover by basic open sets, and establishes that Proj is proper and separated over Spec of the degree-zero component. This construction is fundamental for studying projective varieties and projective schemes in algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| Topology.lean | Defines the topological space ProjectiveSpectrum as relevant homogeneous prime ideals of a graded ring, with the Zariski topology given by zero loci and vanishing ideals |
| StructureSheaf.lean | Constructs the structure sheaf on ProjectiveSpectrum as dependent functions locally expressible as fractions of elements of the same grading, making Proj a locally ringed space |
| Scheme.lean | Proves that Proj is a scheme by constructing homeomorphisms between basic open sets D₊(f) and Spec of the degree-zero part of localizations, using the Gamma-Spec adjunction |
| Basic.lean | Provides basic properties of the scheme Proj A including the structure map to Spec A₀, isomorphisms between basic opens and affine schemes, affine open covers, and stalk isomorphisms |
| Proper.lean | Establishes that Proj 𝒜 is proper and separated over Spec 𝒜₀, completing the geometric properties of the projective spectrum construction |

## Subdirectories

*(No subdirectories)*

## Search Tags

projective-spectrum proj graded-rings homogeneous-ideals zariski-topology structure-sheaf locally-ringed-space scheme affine-cover basic-open-sets localization gamma-spec-adjunction proper-morphisms separated-morphisms algebraic-geometry projective-varieties
