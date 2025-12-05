---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/LocallyConvex
generated: 2025-12-05T02:36:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 17
subdirs_count: 0
---

# LocallyConvex

## Overview

The `LocallyConvex/` directory formalizes the theory of locally convex topological vector spaces (LCTVS), a fundamental class of topological vector spaces whose topology is induced by a family of seminorms. This directory contains definitions and theorems about absorbent and balanced sets, absolutely convex sets and their hulls, von Neumann boundedness, seminorm families, weak topologies (weak dual, weak space, weak operator topology), separation theorems (geometric Hahn-Banach), barrelled spaces, Montel spaces, polar sets, and the strong topology. The material covers both the basic building blocks of local convexity theory and advanced topics like the Banach-Steinhaus theorem and the characterization of continuity via boundedness.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines absorbent and balanced sets, the fundamental building blocks of locally convex spaces; proves that absorbent submodules equal the whole space when the base field is nontrivially normed |
| WithSeminorms.lean | Defines topology induced by families of seminorms; proves that spaces with seminorm-induced topology are locally convex and characterizes boundedness and continuity of linear maps via seminorms |
| AbsConvex.lean | Defines absolutely convex (disked) sets and their hulls; proves that absolutely convex hull equals convex hull of balanced hull |
| AbsConvexOpen.lean | Characterizes topology of locally convex spaces via gauge seminorms of absolutely convex open neighborhoods of zero |
| Bounded.lean | Defines von Neumann boundedness (sets absorbed by all neighborhoods of zero); proves that bounded sets are characterized by sequences and that continuous linear images of bounded sets are bounded |
| BalancedCoreHull.lean | Defines balanced core (largest balanced subset) and balanced hull (smallest balanced superset); proves closed balanced sets form a neighborhood basis |
| Polar.lean | Defines absolute polar sets for bilinear forms; proves polar is closed in weak topology and establishes bipolar theorem |
| Separation.lean | Proves geometric Hahn-Banach separation theorems for disjoint convex sets with various combinations of open/closed/compact assumptions |
| Barrelled.lean | Defines barrelled spaces (spaces where lower semicontinuous seminorms are continuous); proves Banach-Steinhaus theorem (Uniform Boundedness Principle) for pointwise bounded families of continuous linear maps |
| WeakDual.lean | Proves that weak topology induced by a bilinear form is locally convex; gives explicit seminorm family generating the weak topology |
| WeakSpace.lean | Proves that weak closure and strong closure coincide for convex sets in locally convex spaces |
| WeakOperatorTopology.lean | Defines weak operator topology on continuous linear maps; proves WOT is induced by seminorms of the form ‖y(Ax)‖ for dual elements y |
| StrongTopology.lean | Proves that the strong topology (topology of bounded convergence) on spaces of continuous linear maps is locally convex |
| SeparatingDual.lean | Defines typeclass for spaces where continuous linear functionals separate points; proves existence of nontrivial continuous linear operators and transitive action of continuous linear equivalences |
| Montel.lean | Defines Montel spaces (spaces with Heine-Borel property: closed bounded sets are compact); proves normed Montel spaces are finite dimensional and establishes equivalence between compact convergence and strong topology |
| PointwiseConvergence.lean | Proves that topology of pointwise convergence on continuous linear maps is induced by seminorms and is locally convex |
| ContinuousOfBounded.lean | Proves that locally bounded linear maps on first countable spaces are continuous; kept separate to avoid circular imports with operator norm theory |

## Subdirectories

(This is a leaf directory with no subdirectories)

## Search Tags

locally-convex topological-vector-spaces seminorms absorbent balanced absolutely-convex disked von-neumann-bounded barrelled montel weak-topology weak-dual weak-operator-topology strong-topology polar bipolar separation hahn-banach geometric-hahn-banach banach-steinhaus uniform-boundedness seminorm-family gauge-seminorm balanced-hull convex-hull pointwise-convergence bounded-convergence separating-dual lctvs functional-analysis
