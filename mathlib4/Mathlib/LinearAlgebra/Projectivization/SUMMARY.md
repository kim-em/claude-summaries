---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Projectivization
generated: 2026-01-25T22:35:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# Projectivization

## Overview

The `Projectivization/` directory formalizes projective spaces and their geometry. It defines the projectivization ℙ K V of a vector space V over a division ring K as the quotient by scalar equivalence, establishes the bijection with one-dimensional subspaces, and develops the theory of group actions (particularly by the general linear group), cardinality formulas for finite fields, geometric operations (dot product orthogonality and cross product in dimension 3), independence/dependence of points, and the lattice structure of projective subspaces with its correspondence to vector space submodules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: projectivization ℙ K V as quotient by scalar equivalence, constructors (mk from nonzero vector, mk'' from 1-dim submodule), equivalence with one-dimensional subspaces (equivSubmodule), representative selection (rep), submodule correspondence, map operation for semilinear maps, and induction principles |
| Action.lean | Group actions on projectivization: MulAction instance for groups acting K-linearly on V (including general linear group), smul_mk lemma showing g • mk K v = mk K (g • v) |
| Cardinality.lean | Cardinality theory for finite fields: equivalence with quotient by units (equivQuotientOrbitRel), nonzero vectors as product of projectivization and units (nonZeroEquivProjectivizationProdUnits), finiteness conditions, cardinality formulas (Nat.card V - 1 = Nat.card (ℙ k V) * (Nat.card k - 1)), and dimension-dependent formulas (card_of_finrank shows geometric series) |
| Constructions.lean | Geometric constructions in projective space: dot product orthogonality (orthogonal predicate on ℙ F (m → F)), cross product for dimension 3 (cross operation on ℙ F (Fin 3 → F) with convention cross v v = v), orthogonality characterizations, and relationship between equality and vanishing cross product |
| Independence.lean | Independence and dependence of families of points: Independent predicate from linearly independent nonzero vectors, equivalence with lattice-theoretic independence of submodules (independent_iff_iSupIndep), Dependent as negation of Independent, characterization via representatives (dependent_iff shows equivalence with linear dependence of reps), and special case that two points are dependent iff equal |
| Subspace.lean | Subspaces of projective space as lattice: Subspace structure (carrier with closure under addition of representatives), span construction via inductive definition, Galois insertion between sets of points and subspaces, CompleteLattice instance, correspondence with vector space submodules (submodule order equivalence), and membership characterizations (mem_span, span_eq_sInf) |

## Subdirectories

(none)

## Search Tags

projectivization projective-space projective-geometry quotient-by-scalars one-dimensional-subspaces group-actions general-linear-group cardinality finite-fields geometric-series orthogonality dot-product cross-product independence dependence linear-independence projective-subspaces lattice galois-insertion submodule-correspondence
