---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Convex
generated: 2025-12-05T09:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 50
subdirs_count: 3
---

# Convex

## Overview

The `Convex/` directory contains the topological and metric theory of convexity for normed and inner product spaces, extending the purely algebraic/affine convexity results from `Mathlib.Geometry.Convex`. The core content includes fundamental definitions of convex sets and functions, derivatives and second derivative tests for convexity, Jensen's inequality, the Minkowski functional (gauge) as a seminorm, extreme points and the Krein-Milman theorem, Carathéodory's and Radon's theorems, Birkhoff's theorem on doubly stochastic matrices, and various specialized topics (strict/strong/uniform convexity, quasiconvexity, star-convexity, visibility, convex bodies).

Three subdirectories provide specialized theory: `Cone/` develops the topological theory of convex cones with proper cones, dual cones, Farkas' lemma, and separation theorems (Hahn-Banach, M. Riesz extension); `SimplicialComplex/` provides the combinatorial structure of simplicial complexes as downward-closed affine independent vertex sets; and `SpecificFunctions/` contains elementary and derivative-based proofs of convexity/concavity for concrete functions (exp, log, powers, trigonometric functions).

## Key Files

| File | Purpose |
|------|---------|
| README.md | Brief overview noting this folder covers convexity results requiring norms/inner products, referencing Mathlib.Geometry.Convex for metric-free results |
| Basic.lean | Core definitions of convex sets in vector spaces; proves closure under intersections, images, products; provides alternative characterizations via segments and pointwise operations |
| Function.lean | Convex and concave functions (ConvexOn, ConcaveOn); strict variants; proves preservation under composition, addition, suprema |
| Jensen.lean | Finite Jensen's inequality for convex/concave functions; maximum/minimum principles for convex functions on convex hulls |
| Deriv.lean | Relates convexity to derivatives: monotone first derivative implies convex, nonnegative second derivative implies convex; convex functions have monotone derivatives |
| Hull.lean | Convex hull as a closure operator; proves it's the minimal convex set containing a given set |
| Between.lean | Betweenness relation in convex sets; properties of points lying between others |
| BetweenList.lean | Betweenness for lists of points |
| Segment.lean | Line segments `[x -[𝕜] y]` and open segments in vector spaces |
| Combination.lean | Convex combinations and center of mass for finsets |
| Gauge.lean | Minkowski functional (gauge) of a set; when symmetric, convex, and absorbent, it forms a seminorm |
| GaugeRescale.lean | Rescaling properties of the gauge |
| EGauge.lean | Extended gauge taking values in extended reals |
| Topology.lean | Topological properties: interior/closure of convex sets are convex; compactness and closedness of finite convex hulls |
| Strict.lean | Strictly convex sets (open segment between distinct points lies in interior) |
| StrictConvexSpace.lean | Strictly convex normed spaces where the unit ball is strictly convex |
| StrictConvexBetween.lean | Strict convexity with respect to betweenness |
| Strong.lean | Uniformly and strongly convex functions with moduli; m-strongly convex means uniform convexity with modulus m/2 * r^2 |
| Uniform.lean | Uniformly convex spaces (normed spaces with uniform modulus of convexity) |
| Extrema.lean | Extremal points and sets (points that cannot be written as proper convex combinations) |
| Extreme.lean | Extreme points and extreme subsets of convex sets |
| Exposed.lean | Exposed points and exposed faces (extreme sets obtained by maximizing a linear functional) |
| KreinMilman.lean | Krein-Milman lemma (compact sets have extreme points) and theorem (compact convex sets are closures of convex hulls of extreme points) |
| Caratheodory.lean | Carathéodory's theorem on convex hulls in finite-dimensional spaces |
| Radon.lean | Radon's partition theorem |
| Birkhoff.lean | Birkhoff's theorem: doubly stochastic matrices are convex combinations of permutation matrices |
| DoublyStochasticMatrix.lean | Doubly stochastic matrices and their properties |
| Continuous.lean | Continuity properties of convex functions on normed spaces |
| ContinuousLinearEquiv.lean | Preservation of convexity under continuous linear equivalences |
| Integral.lean | Integral versions of Jensen's inequality |
| Measure.lean | Measurability of convex sets |
| Slope.lean | Slopes of convex functions and monotonicity properties |
| Side.lean | Sides of points relative to hyperplanes and affine subspaces |
| Join.lean | Join of convex sets (union of segments between sets) |
| Mul.lean | Multiplicative structure on convex sets |
| Star.lean | Star-convex sets (convex relative to a distinguished center point) |
| StdSimplex.lean | Standard simplex in Euclidean space |
| PartitionOfUnity.lean | Partitions of unity on convex sets |
| PathConnected.lean | Path-connectedness of convex sets |
| Contractible.lean | Contractibility of convex sets |
| Piecewise.lean | Piecewise convex functions |
| Quasiconvex.lean | Quasiconvex functions (sublevel sets are convex) |
| Body.lean | Convex bodies (compact convex sets with nonempty interior) |
| AmpleSet.lean | Ample sets in convex analysis |
| Independent.lean | Independent families of convex sets |
| Intrinsic.lean | Intrinsic interior and closure of convex sets |
| Visible.lean | Visible and locally visible points in convex sets |
| StoneSeparation.lean | Stone's separation theorem for convex sets |
| TotallyBounded.lean | Total boundedness of convex hulls |
| NNReal.lean | Convexity results specific to nonnegative reals |
| LinearIsometry.lean | Preservation of convexity under linear isometries |

## Subdirectories

- [x] `Cone/` - Topological and analytic theory of convex cones; proper cones, dual cones, Farkas' lemma, Hahn-Banach separation
- [x] `SimplicialComplex/` - Simplicial complexes modeled as downward-closed affine independent vertex sets with controlled convex hull intersections
- [x] `SpecificFunctions/` - Convexity/concavity of specific functions: exp, log, rpow, sin, cos, sqrt

## Search Tags

convex convexity convex-sets convex-functions jensen-inequality minkowski-functional gauge extreme-points krein-milman-theorem convex-hull caratheodory birkhoff doubly-stochastic strictly-convex strongly-convex uniformly-convex derivatives second-derivative exposed-points radon segments betweenness star-convex quasiconvex simplex partition-of-unity normed-spaces inner-product-spaces functional-analysis
