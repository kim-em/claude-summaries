---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Module
generated: 2025-12-05T09:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 19
subdirs_count: 5
---

# Module

## Overview

The `Module/` directory provides the core theory of normed vector spaces over normed fields. It defines the fundamental `NormedSpace` typeclass and establishes essential properties including norm-scalar multiplication inequalities, dual spaces, finite-dimensional theory, and the Hahn-Banach theorem. This directory contains both foundational definitions (basic normed space structure, completions, dual spaces) and specialized theory (convexity, connectedness, multilinear maps, tensor products, weak topology). It serves as the bridge between algebraic module theory and topological/metric properties.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `NormedSpace 𝕜 E` requiring `‖a • b‖ ≤ ‖a‖ * ‖b‖`; proves `norm_smul` equality, establishes `NormSMulClass` instance, provides continuity properties of scalar multiplication, discrete topology for integer multiples |
| Dual.lean | Strong dual `StrongDual 𝕜 E` (continuous linear functionals with operator norm topology); inclusion into double dual as bounded linear map and linear isometry; polar sets for functionals |
| WeakDual.lean | Weak-* topology on dual spaces; `WeakDual 𝕜 E` type synonym; continuous mapping `StrongDual → WeakDual`; Banach-Alaoglu theorem (compactness of closed balls/polars in weak-* topology) |
| FiniteDimension.lean | Finite-dimensional normed spaces over complete fields; completeness and properness of finite-dimensional spaces; closedness of finite-dimensional subspaces; norm equivalence via continuous identity maps; Riesz's theorem (compact closed ball implies finite dimension) |
| HahnBanach.lean | Analytic Hahn-Banach extension theorem for continuous linear functionals; extends functionals from subspaces without increasing norm; works over `ℝ` or `ℂ` (via `RCLike`); proves existence of dual vectors with `‖g‖ = 1` and `g x = ‖x‖` |
| Completion.lean | Normed space structure on uniform space completion; `toComplₗᵢ : E →ₗᵢ[𝕜] Completion E` as linear isometry; `toComplL` as continuous linear map; normed algebra structure on completions |
| Complemented.lean | Complemented subspaces (existence of continuous linear projection); equivalence to existence of closed complement; finite codimension subspaces are complemented |
| Convex.lean | Metric properties of convex sets in normed spaces; convexity of norm and distance functions; convex hull preserves boundedness and diameter |
| Connected.lean | Path-connectedness in vector spaces; complement of countable set is path-connected (dimension > 1); sphere path-connectedness; complement of low-codimension subspace is path-connected |
| Ray.lean | `SameRay` predicate in real normed spaces; triangle equality `‖x + y‖ = ‖x‖ + ‖y‖` for vectors in same ray; `‖x‖ • y = ‖y‖ • x` characterization; uniqueness of unit vector in ray |
| RieszLemma.lean | Riesz's lemma: for closed proper subspace `F`, exists `x` with `‖x - F‖ ≥ r * ‖x‖` for any `r < 1`; stronger version with controlled norm and distance guarantees for nontrivially normed fields |
| MStructure.lean | L-projections (‖x‖ = ‖P x‖ + ‖(1-P) x‖) and M-projections (‖x‖ = max(‖P x‖, ‖(1-P) x‖)); Boolean algebra structure for L-projections; foundational theory for M-ideals and summands |
| Extr.lean | Extremal points and local extrema in normed spaces related to convex sets |
| Normalize.lean | Normalization operations for vectors in normed spaces |
| Shrink.lean | Techniques for shrinking sets while preserving norm properties |
| Span.lean | Span and closure properties in normed modules |
| TransferInstance.lean | Instance transfer mechanisms for normed space structures |
| ENormedSpace.lean | (Deprecated) Extended norms (taking value `∞`) on vector spaces; `EMetricSpace` structure; finite-norm subspace with induced `NormedSpace` structure; superseded by `ENormed(Add)(Comm)Monoid` classes |
| MultipliableUniformlyOn.lean | Uniform convergence of infinite products `∏' i, (1 + f i x)` for complex-valued function sequences; `hasSumUniformlyOn` for logarithms; composition with exponential preserving uniform convergence |

## Subdirectories

- [x] `Alternating/` - Alternating multilinear maps (alternating tensor algebra, antisymmetric operations) (complete)
- [x] `Ball/` - Balls in normed spaces (pointwise operations, convexity properties, ball-specific results) (complete)
- [x] `Multilinear/` - Continuous multilinear maps with operator norm theory; currying/uncurrying operations and linear isometric equivalences (complete)
- [x] `PiTensorProduct/` - Pi-type tensor products with projective and injective seminorms; universal property as isometric linear equivalence (complete)
- [x] `RCLike/` - Real-closed-like fields (ℝ and ℂ); unified treatment of normed spaces over these fields (complete)

## Search Tags

normed-spaces normed-modules vector-spaces scalar-multiplication norm-smul dual-spaces strong-dual weak-dual banach-alaoglu double-dual hahn-banach extension-theorem finite-dimensional riesz-lemma complemented-subspaces completions convex-sets path-connected same-ray l-projections m-projections multilinear-maps tensor-products rclike functional-analysis continuous-linear-functionals operator-norm weak-star-topology polars isometry
