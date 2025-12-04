---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Vertex
generated: 2025-12-04T06:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Vertex

## Overview

The `Vertex/` directory contains foundational theory for vertex operators and vertex algebras, algebraic structures that play a central role in conformal field theory and the mathematical study of the Monster group. The directory provides both heterogeneous and homogeneous formulations of vertex operators as R-linear maps to Hahn series (generalizations of Laurent series), with coefficients, composition operations, and construction methods from coefficient functions.

## Key Files

| File | Purpose |
|------|---------|
| HVertexOperator.lean | Defines heterogeneous vertex operators `HVertexOperator Γ R V W` as R-linear maps from V to Γ-indexed Hahn series with coefficients in W, with coefficient extraction, composition of vertex operators via iterated Hahn series on lexicographic product orders, and construction from coefficient functions satisfying partially well-ordered support conditions |
| VertexOperator.lean | Defines (homogeneous) vertex operators `VertexOperator R V` as specialization of heterogeneous case with Γ=ℤ and V=W, introduces normalized coefficient indexing `A[[n]]` corresponding to coefficient at `-n-1`, provides construction from endomorphism-valued functions satisfying bounded-pole conditions, and serves as main entry point for standard vertex operator theory |

## Subdirectories

*(none)*

## Search Tags

vertex-operator vertex-algebra hahn-series laurent-series conformal-field-theory meromorphic-field composition heterogeneous-vertex-operator normalized-coefficients bounded-pole-condition
