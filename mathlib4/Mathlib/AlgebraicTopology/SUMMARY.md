---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 7
subdirs_count: 10
---

# AlgebraicTopology

## Overview

The `AlgebraicTopology/` directory contains formalized algebraic topology theory, including the fundamental constructions for computing homology and homotopy invariants of topological spaces. The directory covers simplicial methods (simplicial sets, simplicial objects, and the simplex category), homological algebra constructions (Moore complex, alternating face map complex, and the Dold-Kan correspondence), and fundamental groups/groupoids. It also includes the bridge between topology and combinatorics via the singular set functor and geometric realization, as well as specialized topics like Čech nerves, quasicategories, and model categories.

## Key Files

| File | Purpose |
|------|---------|
| AlternatingFaceMapComplex.lean | Constructs the alternating face map complex functor from simplicial objects to chain complexes, where differentials are alternating sums of face maps; includes the dual cochain version and natural transformation from the Moore complex |
| CechNerve.lean | Defines the Čech nerve and augmented Čech nerve of an arrow as simplicial objects, constructed via iterated wide pullbacks; includes the special case for arrows to terminal objects (important for group cohomology) |
| MooreComplex.lean | Constructs the normalized Moore complex functor from simplicial objects to chain complexes in abelian categories, with n-th object as intersection of kernels of degeneracy maps and differentials induced from the 0-th face map |
| SimplicialNerve.lean | Defines the simplicial nerve (homotopy coherent nerve) of a simplicial category via simplicial thickening and enriched functors; framework for relating simplicial categories to quasicategories |
| ExtraDegeneracy.lean | Formalizes the notion of extra degeneracy for augmented simplicial objects (a formal "σ(-1)"), used to prove contractibility of connected components; shows extra degeneracies induce homotopy equivalences on alternating face map complexes |
| SingularSet.lean | Defines the singular simplicial set functor from topological spaces to simplicial sets and its left adjoint geometric realization functor; provides the fundamental adjunction between topology and combinatorial homotopy theory |
| TopologicalSimplex.lean | Defines the standard topological n-simplex as convex combinations in ℝⁿ⁺¹ and the functor from SimplexCategory to TopCat; foundational for the singular set construction |

## Subdirectories

- [x] `DoldKan/` - The Dold-Kan correspondence between simplicial objects in abelian categories and chain complexes (complete)
- [ ] `FundamentalGroupoid/` - Fundamental groupoid construction and fundamental group theory (pending)
- [ ] `ModelCategory/` - Model category structures on simplicial sets and related categories (pending)
- [ ] `Quasicategory/` - Quasicategory (∞-category) theory via simplicial sets (pending)
- [ ] `RelativeCellComplex/` - Relative cell complexes and CW-complex theory (pending)
- [ ] `SimplexCategory/` - The simplex category Δ (finite non-empty linear orders and order-preserving maps) (pending)
- [ ] `SimplicialCategory/` - Simplicial categories (categories enriched over simplicial sets) (pending)
- [ ] `SimplicialObject/` - General theory of simplicial objects in arbitrary categories (pending)
- [ ] `SimplicialSet/` - Simplicial sets as presheaves on the simplex category (pending)
- [ ] `SingularHomology/` - Singular homology theory for topological spaces (pending)

## Search Tags

algebraic-topology simplicial-sets simplicial-objects homology homotopy fundamental-group fundamental-groupoid chain-complex moore-complex alternating-face-map-complex dold-kan cech-nerve singular-set geometric-realization simplex-category simplicial-category quasicategory model-category extra-degeneracy topological-simplex
