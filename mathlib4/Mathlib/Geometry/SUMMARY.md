---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry
generated: 2026-01-24T23:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 0
subdirs_count: 5
---

# Geometry

## Overview

The `Geometry/` directory provides a comprehensive formalization of geometric structures across the mathematical spectrum, from classical Euclidean geometry to modern differential and algebraic geometry. The directory's five major branches represent distinct yet interconnected geometric paradigms:

**Euclidean geometry** (`Euclidean/`) delivers classical synthetic geometry in real inner product spaces, including complete theories of simplices (circumcenters, incenters, altitudes, Monge points), triangle congruence (SSS, SAS, ASA, AAS) and similarity (AA, SAS), angle theory (both oriented and unoriented), sphere geometry with Ptolemy's theorem (Freek #95) and intersecting chords (Freek #55), and geometric inversion. This implements the geometric intuitions underlying compass-and-straightedge constructions in a coordinate-free framework.

**Convex geometry** (`Convex/`) works at a purely algebraic level without topology or norms, formalizing convex cones with complete lattice structure, dual cones via bilinear pairings, tensor products of pointed cones, and the correspondence between cones and ordered modules. This provides the algebraic foundations complementing the topological convexity theory in Analysis.

**Differential geometry** (`Manifold/`) constitutes the most extensive component, building smooth manifolds on structure groupoids, charted spaces, and models with corners. It includes the full smoothness infrastructure (`ContMDiff`), manifold derivatives (`mfderiv`), diffeomorphisms, immersions, smooth embeddings, bump functions and partitions of unity, vector bundles (including tangent bundles), Riemannian metrics, Lie groups and Lie algebras, integral curves of vector fields, the Whitney embedding theorem, and the sheaf of smooth functions making manifolds into locally ringed spaces.

**Geometric group theory** (`Group/`) formalizes the study of finitely generated groups through their geometric actions, proving fundamental growth results: infinite groups have at least linear growth, with multiplicative relationships between group growth, quotient growth, and normal subgroup intersections.

**Algebraic geometry foundations** (`RingedSpace/`) provides the complete categorical infrastructure needed for schemes, defining the hierarchy from presheafed spaces through sheafed spaces, ringed spaces, to locally ringed spaces with local ring stalks. This includes morphisms, open immersions, gluing constructions, colimits, stalks, and residue fields.

Together, these components form a unified geometric framework connecting classical geometric intuitions with modern categorical, differential, and algebraic perspectives—from ruler-and-compass constructions to schemes and smooth manifolds.

## Key Files

No files directly in this directory.

## Subdirectories

- [x] `Convex/` - Convex geometry without norms or inner products (cones and convex sets)
- [x] `Euclidean/` - Euclidean geometry: real inner product spaces, affine Euclidean spaces, angles, circumcenters, incenters, altitudes, perpendicular bisectors, congruence, similarity, simplices, spheres, triangles, signed distances, Monge points, projections, and inversions
- [x] `Group/` - Geometric group theory: finitely generated groups acting on geometric spaces, group growth
- [x] `Manifold/` - Differential geometry: smooth manifolds with charted spaces, atlases, structure groupoids, smooth maps (ContMDiff), diffeomorphisms, local coordinates, tangent bundles, bump functions, immersions, Lie groups and Lie algebras, bordism theory, conformal structures, integral curves
- [x] `RingedSpace/` - Algebraic geometry foundations: ringed spaces as sheafed spaces with commutative rings, locally ringed spaces, presheafed spaces, open immersions, stalks, gluing theory, colimits, residue fields

## Search Tags

geometry euclidean-geometry convex-geometry differential-geometry manifolds smooth-manifolds ringed-spaces locally-ringed-spaces sheafed-spaces geometric-group-theory inner-product affine-space simplex circumcenter angle sphere triangle diffeomorphism charted-space atlas tangent-bundle lie-group algebraic-geometry
