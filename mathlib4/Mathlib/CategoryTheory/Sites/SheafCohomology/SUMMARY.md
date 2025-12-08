---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sites/SheafCohomology
generated: 2025-12-08T14:35:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# SheafCohomology

## Overview

The `SheafCohomology/` directory provides the formalization of sheaf cohomology theory for abelian sheaves on Grothendieck sites. It defines cohomology groups as Ext-groups between the constant sheaf with values ℤ and a given abelian sheaf, and introduces the cohomology presheaf that computes local cohomology at each object. This implements the categorical/derived functor approach to sheaf cohomology as used in modern algebraic geometry and homological algebra.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core sheaf cohomology definitions: `Sheaf.H F n` as Ext-groups from constant ℤ-sheaf to abelian sheaf F, and `cohomologyPresheaf F n` computing local cohomology via free abelian sheaves |

## Subdirectories

*(none)*

## Search Tags

sheaf-cohomology ext-groups grothendieck-topology abelian-sheaves derived-functors constant-sheaf cohomology-presheaf homological-algebra algebraic-geometry
