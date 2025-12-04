---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/SimplicialSet/AnodyneExtensions
generated: 2025-12-04T08:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# AnodyneExtensions

## Overview

The `AnodyneExtensions/` directory provides a complete combinatorial characterization of strong (inner) anodyne extensions for simplicial sets, following Sean Moss's approach. The theory centers on "pairings" - partitions of nondegenerate simplices into type (I) and type (II) simplices with a bijection between them. This captures the essential structure of transfinite compositions of horn inclusions: when attaching a simplex along a horn, exactly two nondegenerate simplices are added (the simplex itself as type I, and the unique missing face as type II). The directory establishes foundational predicates (uniquely codimensional faces), core pairing structures with helper constructions (PairingCore), rank functions for proving well-foundedness, and regularity conditions that characterize strong anodyne extensions.

## Key Files

| File | Purpose |
|------|---------|
| IsUniquelyCodimOneFace.lean | Defines the predicate that a simplex is uniquely a 1-codimensional face of another simplex (unique i such that X.δ i y = x), foundational for proper pairings |
| Pairing.lean | Defines pairings as partitions of nondegenerate simplices not in a subcomplex into type (I) and (II) with a bijection between them; establishes proper, inner, and regular pairings with ancestrality relations |
| PairingCore.lean | Helper structure for constructing pairings using an index type ι and dimension function, allowing definitional control over simplex dimensions; provides equivalence with Pairing structure |
| Rank.lean | Defines (weak) rank functions from pairing indices to partially ordered types that map ancestrality relations to strict inequalities, used to prove regularity by establishing well-foundedness of ancestral relations |

## Subdirectories

*(No subdirectories)*

## Search Tags

anodyne-extensions strong-anodyne inner-anodyne horn-inclusions pairings type-I-simplices type-II-simplices proper-pairing regular-pairing ancestral-relation rank-functions well-foundedness codimensional-faces model-category moss-2020 kan-quillen simplicial-sets nondegenerate-simplices
