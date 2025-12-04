---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/Quasicategory
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Quasicategory

## Overview

The `Quasicategory/` directory contains the formalization of quasicategory (∞-category) theory via simplicial sets. Quasicategories are simplicial sets satisfying inner horn-filling conditions, providing a common model for infinity categories. The directory establishes the core definition, proves that strict Segal simplicial sets and Kan complexes are quasicategories, shows that the nerve of any category is a quasicategory, constructs a strict bicategory structure on the category of quasicategories, and develops the theory of 2-truncated quasicategories with their homotopy relations and homotopy categories.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines quasicategories as simplicial sets satisfying inner horn-filling conditions (0 < i < n); proves every Kan complex is a quasicategory |
| StrictSegal.lean | Proves that any simplicial set satisfying the strict Segal condition (simplices uniquely determined by their spine) is a quasicategory |
| Nerve.lean | Shows that the nerve of any category is a quasicategory by virtue of satisfying the strict Segal condition |
| StrictBicategory.lean | Constructs the strict bicategory `QCat.strictBicategory` whose objects are quasicategories, 1-morphisms are maps of simplicial sets, and 2-morphisms are homotopy classes of homotopies |
| TwoTruncated.lean | Defines 2-truncated quasicategories via three horn-filling properties; establishes left and right homotopy relations as equivalence relations that coincide; constructs the homotopy category `HomotopyCategory₂` with morphisms given by homotopy classes of edges |

## Subdirectories

(none)

## Search Tags

quasicategory infinity-category simplicial-set horn-filling inner-horn kan-complex strict-segal nerve bicategory homotopy-category homotopy-relation 2-truncated kerodon composition
