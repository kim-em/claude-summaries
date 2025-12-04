---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/RelativeCellComplex
generated: 2025-12-04T18:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# RelativeCellComplex

## Overview

The `RelativeCellComplex/` directory formalizes the theory of relative cell complexes in abstract category theory. It provides a framework for describing morphisms that are built by transfinitely composing "cell attachment" operations, where cells are specified by a family of morphisms. This abstraction generalizes classical CW-complexes (where n-disks are attached at the n-th step) and is fundamental to the small object argument in homotopy theory. The directory contains two files: one defining the cell attachment operation as a pushout of coproducts, and another defining relative cell complexes as transfinite compositions of such operations.

## Key Files

| File | Purpose |
|------|---------|
| AttachCells.lean | Defines the `AttachCells` structure expressing that a morphism `f : X₁ ⟶ X₂` is obtained by attaching cells from a family `g a : A a ⟶ B a` via a pushout diagram with coproducts; includes reindexing operations and equivalence with the pushouts-of-coproducts morphism property |
| Basic.lean | Defines `RelativeCellComplex` as a transfinite composition of morphisms with `AttachCells` structures, allowing different cell families at each step; includes the `Cells` index type, cell inclusions, and extensionality principles; used in CW-complex formalization and the small object argument |

## Subdirectories

*(none)*

## Search Tags

relative-cell-complex cell-attachment transfinite-composition pushout coproduct categorical-homotopy-theory small-object-argument cw-complex abstract-topology morphism-property well-founded-recursion colimit
