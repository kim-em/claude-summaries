---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Groupoid
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 6
subdirs_count: 0
---

# Groupoid

## Overview

The `Groupoid/` directory contains specialized constructions and properties for groupoids (categories where all morphisms are isomorphisms). It provides basic properties (thinness, total disconnectedness), the vertex group construction (isotropy groups at objects), free groupoid constructions on both quivers and categories, subgroupoid theory with normality conditions, and the discrete groupoid instance. This extends the core groupoid definition in the parent directory with structural results and universal properties.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Basic properties including thin groupoids and totally disconnected subgroupoids |
| Discrete.lean | Groupoid instance for discrete categories (all morphisms are identities) |
| VertexGroup.lean | Vertex group (isotropy group) at an object as a group structure on endomorphisms with conjugation isomorphisms |
| FreeGroupoid.lean | Free groupoid on a quiver via symmetrification and quotient by reduction relation with universal property |
| FreeGroupoidOfCategory.lean | Free groupoid on a category as localization inverting all morphisms, with adjunction between Grpd and Cat |
| Subgroupoid.lean | Subgroupoids as arrow subsets closed under composition and inversion with lattice structure and normality |

## Subdirectories

*(none)*

## Search Tags

groupoid category-theory free-groupoid vertex-group isotropy-group subgroupoid normal-subgroupoid discrete-category universal-property localization adjunction quiver symmetrification
