---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Category
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Category

## Overview

The `Category/` subdirectory provides the categorical formulation of measurable spaces, defining `MeasCat` as the category of measurable spaces with measurable functions as morphisms. It formalizes the Giry monad (the `Measure` functor that sends a measurable space to the space of measures on it), proves that the nonnegative Lebesgue integral forms an algebra over this monad, and defines the Borel functor that canonically embeds topological spaces into measurable spaces by equipping them with their Borel σ-algebra.

## Key Files

| File | Purpose |
|------|---------|
| MeasCat.lean | Defines the category of measurable spaces (`MeasCat`), the Giry monad (monadic structure on the `Measure` functor with Dirac measure as unit and measure join as multiplication), proves the Lebesgue integral is a Giry algebra, and defines the Borel functor embedding `TopCat` into `MeasCat` |

## Subdirectories

*(No subdirectories)*

## Search Tags

category-theory measurable-space meascat giry-monad measure-functor borel-functor concrete-category markov-kernel probability-kernel dirac-measure measure-join lebesgue-integral monad-algebra topological-space
