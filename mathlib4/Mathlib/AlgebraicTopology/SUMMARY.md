---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology
generated: 2025-12-04T17:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 10
---

# AlgebraicTopology

## Overview

The `AlgebraicTopology/` directory provides a comprehensive formalization of algebraic topology, implementing both the classical computational machinery and modern categorical foundations of the subject. The core architecture builds from the simplex category Δ (with multiple equivalent perspectives including generators-and-relations and monoidal structure on augmentations) to general simplicial objects in arbitrary categories, then specializes to simplicial sets as Type-valued presheaves. The directory establishes the fundamental Dold-Kan correspondence—an equivalence between simplicial objects and chain complexes in abelian categories—using an innovative approach via idempotent completions that constructs projection endomorphisms identifying the normalized Moore complex as a formal direct factor. For topological spaces, it provides the singular set functor and its left adjoint geometric realization, enabling the computation of singular homology with coefficients in arbitrary preadditive categories. The fundamental groupoid construction yields fundamental groups via vertex groups, with complete functoriality and product preservation. Advanced structures include model category theory with fibrations, cofibrations, and weak equivalences satisfying Quillen's axioms (featuring Brown's lemma, Whitehead theorem, and Joyal's trick), quasicategory (∞-category) theory via simplicial sets with inner horn-filling conditions, and the categorical framework for relative cell complexes supporting CW-complex theory and the small object argument. The directory also includes specialized constructions like Čech nerves for cohomology, extra degeneracies for proving contractibility, and simplicial nerves for relating simplicial categories to quasicategories.

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
- [x] `FundamentalGroupoid/` - Fundamental groupoid construction and fundamental group theory (complete)
- [x] `ModelCategory/` - Model category structures on simplicial sets and related categories (complete)
- [x] `Quasicategory/` - Quasicategory (∞-category) theory via simplicial sets (complete)
- [x] `RelativeCellComplex/` - Relative cell complexes and CW-complex theory (complete)
- [x] `SimplexCategory/` - The simplex category Δ (finite non-empty linear orders and order-preserving maps) (complete)
- [x] `SimplicialCategory/` - Simplicial categories (categories enriched over simplicial sets) (complete)
- [x] `SimplicialObject/` - General theory of simplicial objects in arbitrary categories (complete)
- [x] `SimplicialSet/` - Simplicial sets as presheaves on the simplex category (complete)
- [x] `SingularHomology/` - Singular homology theory for topological spaces (complete)

## Search Tags

algebraic-topology simplicial-sets simplicial-objects homology homotopy fundamental-group fundamental-groupoid chain-complex moore-complex alternating-face-map-complex dold-kan cech-nerve singular-set geometric-realization simplex-category simplicial-category quasicategory model-category extra-degeneracy topological-simplex
