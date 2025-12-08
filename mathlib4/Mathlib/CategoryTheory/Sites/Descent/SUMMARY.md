---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sites/Descent
generated: 2025-12-08T06:36:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Descent

## Overview

The `Descent/` directory formalizes descent theory for pseudofunctors from locally discrete opposite categories to Cat, providing the categorical framework for gluing data over covering families. It defines descent data (objects over each member of a family equipped with compatibility isomorphisms over pullbacks) and the prestack condition (descent of morphisms), which requires that presheaves of homomorphisms between pulled-back objects are sheaves. This machinery is fundamental for stack theory and for understanding when local data can be uniquely glued into global objects.

## Key Files

| File | Purpose |
|------|---------|
| IsPrestack.lean | Prestack typeclass: pseudofunctors satisfying descent of morphisms (presheaves of Hom sets are sheaves for a Grothendieck topology) with presheafHom and sheafHom constructions |
| DescentData.lean | Category of descent data: objects over a family of morphisms with compatibility isomorphisms, including ofObj constructor, toDescentData functor, and infrastructure for morphisms of descent data |

## Subdirectories

None.

## Search Tags

descent-theory prestacks descent-data pseudofunctors locally-discrete gluing-conditions compatibility-isomorphisms sheaf-of-morphisms stack-theory fibered-categories giraud effective-descent
