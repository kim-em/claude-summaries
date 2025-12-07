---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/GuitartExact
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# GuitartExact

## Overview

The `GuitartExact/` directory formalizes Guitart exact squares, a category-theoretic notion that generalizes various categorical concepts including fully faithful functors, adjunctions, and final/initial functors. A 2-square consisting of four functors T, L, R, B and a natural transformation `w : T ⋙ R ⟶ L ⋙ B` is Guitart exact if certain auxiliary categories of structured arrows are connected. This theory plays a crucial role in the characterization of pointwise Kan extensions and will be used in the construction of derived functors.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `GuitartExact` typeclass for 2-squares with equivalence characterizations via finality, initiality, and connectedness of auxiliary categories |
| KanExtension.lean | Relationship between Guitart exact squares and pointwise Kan extensions, showing base change isomorphisms for left Kan extensions |
| Opposite.lean | Proves that a 2-square is Guitart exact if and only if its opposite (transposed) 2-square is Guitart exact |
| Over.lean | Shows that the natural square involving `Over.post F` and `Over.forget` functors is Guitart exact when binary products exist and are preserved |
| VerticalComposition.lean | Proves that vertical composition of Guitart exact squares is Guitart exact, with support for whiskering by natural isomorphisms |

## Subdirectories

(none)

## Search Tags

category-theory guitart-exact-squares kan-extensions derived-functors final-functors initial-functors structured-arrows costructured-arrows two-squares pointwise-kan-extension base-change vertical-composition over-categories
