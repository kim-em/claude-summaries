---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Group
generated: 2025-12-05T10:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 31
subdirs_count: 1
---

# Group

## Overview

The `Group/` directory provides the complete foundational theory of normed (additive) groups and seminormed groups in mathlib4. It establishes the fundamental typeclasses (`SeminormedAddGroup`, `NormedAddGroup`, `SeminormedAddCommGroup`, `NormedAddCommGroup`) and their relationship to metric space structures where distance is given by `dist x y = ‖x - y‖`. The directory encompasses both the algebraic perspective (bounded homomorphisms `NormedAddGroupHom`, quotient norms, completeness criteria) and the categorical perspective (the `SemiNormedGrp` category with kernels, cokernels, and completion functors). Specialized topics include ultrametric/nonarchimedean norms, infinite series and summability, function spaces with uniform/normal convergence, and normed structures on specific mathematical objects (integers, rationals, additive circles, additive torsors).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions for normed groups: `Norm`, `NNNorm`, `ENorm` classes; `SeminormedAddGroup`, `NormedAddGroup`, and their commutative variants; defines 10 core typeclass hierarchies for (semi)normed (commutative) groups; establishes metric space structure compatible with group operations (`dist x y = ‖x - y‖`) |
| Seminorm.lean | Defines group seminorms as structure types: `AddGroupSeminorm`, `GroupSeminorm`, `NonarchAddGroupSeminorm`, `AddGroupNorm`, `GroupNorm`; provides bare functions with axioms (subadditivity, positivity, negation-invariance) before bundling into typeclasses |
| Hom.lean | Bounded group homomorphisms (`NormedAddGroupHom`): morphisms between seminormed groups with boundedness condition (`∃ C, ‖f v‖ ≤ C * ‖v‖`); relates boundedness to continuity and Lipschitz continuity; provides normed group structure on hom types; constructions like kernel, range, equalizer |
| Quotient.lean | Quotient norms for seminormed groups: `SeminormedAddCommGroup` and `NormedAddCommGroup` instances on `M ⧸ S` for subgroups `S`; norm defined as infimum over coset representatives; universal property via `lift`; `IsQuotient` predicate; extends to quotients of modules by submodules and rings by ideals |
| Constructions.lean | Normed group instances for type constructors: `PUnit` (trivial norm), `ULift` (inherited norm), finite products with infinity norm |
| Ultra.lean | Ultrametric norms and nonarchimedean groups: equivalence between ultrametric distance and nonarchimedean norm (`‖x + y‖ ≤ max ‖x‖ ‖y‖`); instances for nonarchimedean topological groups; finite sum norm properties |
| InfiniteSum.lean | Summability and infinite series in normed groups: `summable_iff_vanishing_norm`, comparison tests (`Summable.of_norm_bounded`), norm bounds on tsums (`tsum_of_norm_bounded`); versions for `nnnorm` and `enorm` |
| Completeness.lean | Completeness criterion for normed groups: `NormedAddCommGroup.completeSpace_of_summable_imp_tendsto` shows a normed group is complete iff absolutely convergent series converge |
| Uniform.lean | Uniform structure properties: relates uniformity to norm topology; uniform continuity of group operations; Cauchy sequences in normed groups |
| SemiNormedGrp.lean | Categorical structure: defines category `SemiNormedGrp` of seminormed abelian groups with bounded homomorphisms as morphisms; concrete category instance |
| Bounded.lean | Theory of bounded sets in normed groups: characterization via norm bounds, closure properties, relationship to metric bounded sets |
| Hom­Completion.lean | Extension of normed group homomorphisms to completions: universal property for continuous maps between completions |
| AddTorsor.lean | Normed additive torsors: affine spaces with compatible norm structure; distance induced by norm on difference space |
| AddCircle.lean | Normed group structure on `AddCircle p` (ℝ modulo period `p`): quotient norm from ℝ by discrete subgroup, characterization of norm as distance to nearest multiple |
| Pointwise.lean | Pointwise operations on sets in normed groups: norm bounds for sums, scalar multiples, and convex combinations of sets |
| Continuity.lean | Continuity properties: norm as continuous function, continuous scalar multiplication in normed spaces, open/closed ball properties |
| Subgroup.lean | Normed structures on subgroups: induced seminorm on additive subgroups, compatibility with ambient group norm |
| Submodule.lean | Brief results about submodules in normed contexts (connects to module theory) |
| ControlledClosure.lean | Controlled closure in normed groups: closure operations respecting norm bounds |
| SeparationQuotient.lean | Separation quotient: quotient by elements of norm zero to get a normed space from a seminormed space |
| Indicator.lean | Indicator functions in normed groups: norm estimates for indicator functions on sets |
| Tannery.lean | Tannery's theorem: dominated convergence for series in normed groups |
| FunctionSeries.lean | Convergence of function series: uniform convergence, normal convergence, relation to summability of norms |
| Lemmas.lean | Miscellaneous auxiliary lemmas about norms in groups |
| BallSphere.lean | Properties specific to balls and spheres in normed groups |
| CocompactMap.lean | Cocompact maps between normed groups: maps where preimages of compact sets are compact |
| ZeroAtInfty.lean | Functions vanishing at infinity in normed groups |
| Completion.lean | Completion of normed groups: universal property, functoriality |
| NullSubmodule.lean | Null submodules: submodules consisting of elements with norm zero |
| Int.lean | Normed group structure on integers: standard absolute value norm |
| Rat.lean | Normed group structure on rationals: standard absolute value norm |

## Subdirectories

- [x] `SemiNormedGrp/` - Categorical infrastructure: the `SemiNormedGrp` and `SemiNormedGrp₁` (norm-nonincreasing) categories as concrete categories; kernels and cokernels with norm-preserving properties; completion as an additive endofunctor with universal property for extending morphisms to complete spaces

## Search Tags

normed-groups seminormed-groups additive-groups norms seminorms bounded-homomorphisms normed-homs quotient-norms ultrametric nonarchimedean infinite-sums summability completeness uniform-structure categorical-structures seminormedgrp bounded-sets additive-torsors add-circle group-seminorms positive-definite metric-spaces pseudometric-spaces cauchy-sequences function-series dominated-convergence
