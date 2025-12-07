---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Distributive
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Distributive

## Overview

The `Distributive/` directory contains the formalization of distributive categories in category theory, where tensor products distribute over coproducts. It provides two main concepts: monoidal distributive categories (where left/right tensor functors preserve binary coproducts) and Cartesian distributive categories (Cartesian monoidal categories that are also monoidal distributive). The theory includes key results such as the equivalence of left and right distributivity in symmetric categories, automatic distributivity in closed monoidal categories and preadditive categories, and the monicity of coproduct coprojections in Cartesian distributive categories.

## Key Files

| File | Purpose |
|------|---------|
| Monoidal.lean | Core theory of monoidal distributive categories including left/right distributivity classes, distributivity isomorphisms `∂L` and `∂R`, proofs that closed monoidal and preadditive categories are distributive, and instance for endofunctor categories |
| Cartesian.lean | Specialization to Cartesian distributive categories defined as Cartesian monoidal categories with monoidal distributivity, including proof that coproduct coprojections are monic |

## Subdirectories

None.

## Search Tags

category-theory distributive-categories monoidal-categories cartesian-categories tensor-products coproducts distributivity-isomorphisms closed-monoidal preadditive-categories symmetric-monoidal
