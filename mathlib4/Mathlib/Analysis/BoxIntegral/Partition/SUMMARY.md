---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/BoxIntegral/Partition
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# Partition

## Overview

The `Partition/` directory contains the formalization of partitions and tagged partitions of rectangular boxes in ℝⁿ, which form the foundation for box-based integration theories (Riemann, Henstock-Kurzweil, McShane). This directory defines prepartitions (finite sets of pairwise disjoint subboxes) and partitions (prepartitions that cover the entire box), tagged partitions (partitions with a distinguished point in each box), operations on partitions (splitting along hyperplanes, binary unions, restrictions), filters for defining different integration theories based on partition properties, and box-additive functions (functions satisfying f(J) = Σ f(Jᵢ) for any partition of J).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `Prepartition` (finite pairwise disjoint subboxes) and `IsPartition` predicate (prepartition covering entire box); defines operations: `single` (singleton partition), `biUnion` (hierarchical composition), `restrict` (to subbox), `filter` (by predicate), `disjUnion` (binary union); proves semilattice structure with inf, partial order, and distortion bounds |
| Tagged.lean | Defines `TaggedPrepartition` extending `Prepartition` with tagged points; defines `IsHenstock` (tags in own boxes), `IsSubordinate` (boxes in balls around tags), `biUnionTagged` and `biUnionPrepartition` for hierarchical composition, `infPrepartition` for combining tagged and untagged partitions; proves tag uniqueness bounds (≤2ⁿ boxes per tag) and distortion properties |
| Filter.lean | Defines `IntegrationParams` structure encoding 8 integration theories via Boolean flags (bRiemann: constant vs position-dependent bounds; bHenstock: tags in own boxes; bDistortion: distortion constraints); defines four well-known theories (Riemann, Henstock, McShane, GP=⊥); constructs filters `toFilter`, `toFilterDistortion`, `toFilteriUnion` via `MemBaseSet` predicate combining subordination, Henstock, and distortion constraints; proves filter properties and basis theorems |
| Split.lean | Defines splitting boxes along hyperplanes: `splitLower I i x` and `splitUpper I i x` split box I along {y \| y i = x} into two pieces (as `WithBot (Box ι)`); `Prepartition.split I i a` creates 2-element partition from split; `Prepartition.splitMany I s` splits along multiple hyperplanes in finite set s; proves `exists_iUnion_eq_diff`: any prepartition π admits complement prepartition covering I \ π.iUnion |
| SubboxInduction.lean | Infrastructure for inductive reasoning on boxes via splitting; defines predicates and provides induction principles for proving properties about all subboxes by recursively splitting along hyperplanes (file content not read in detail) |
| Additive.lean | Defines `BoxAdditiveMap`: functions f : Box ι → M satisfying f(J) = Σ f(Jᵢ) for any partition {Jᵢ} of J; provides type class instances (Zero, Add, SMul) and proves additive maps form a module; used to model measure and integral as box-additive functions |
| Measure.lean | Proves boxes and their closures are measurable sets; proves locally finite measures have finite measure on boxes; defines `Measure.toBoxAdditive` bundling μ.real as box-additive function; proves `volume_apply`: volume of box = ∏ᵢ (upper i - lower i); defines `BoxAdditiveMap.volume` as scalar multiplication operator |

## Subdirectories

None.

## Search Tags

partition prepartition tagged-partition box-integral henstock riemann mcshane integration-params filter box-additive measure splitting hyperplane distortion subordinate prepartition-operations semilattice box-splitting volume

