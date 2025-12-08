---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Topos
generated: 2025-12-08T15:39:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# Topos

## Overview

The `Topos/` directory contains the formalization of subobject classifiers, one of the fundamental defining features of elementary topoi in category theory. A subobject classifier is a categorical generalization of the notion of truth values, providing a universal way to characterize subobjects (monomorphisms) via characteristic maps. The directory currently implements the equivalence between having a subobject classifier and the representability of the subobjects presheaf, a key result from topos theory. This forms the foundation for the categorical study of topoi, which generalize the category of sets and sheaves.

## Key Files

| File | Purpose |
|------|---------|
| Classifier.lean | Defines subobject classifiers (`Classifier C` structure), truth morphisms `truth : Ω₀ ⟶ Ω`, characteristic maps `χ m` for monomorphisms, pullback characterization of subobjects, and proves the fundamental equivalence theorem that a category has a subobject classifier iff the subobjects presheaf is representable |

## Subdirectories

*(No subdirectories)*

## Search Tags

topos subobject-classifier truth-morphism characteristic-map representable-functor subobjects-presheaf elementary-topos pullback-squares regular-monomorphism balanced-category grothendieck-topos sheaves
