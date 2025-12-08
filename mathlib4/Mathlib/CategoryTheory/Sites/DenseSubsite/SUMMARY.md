---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sites/DenseSubsite
generated: 2025-12-08T06:43:22Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# DenseSubsite

## Overview

The `DenseSubsite/` directory formalizes dense subsites in Grothendieck topology, where a functor `G : C ⥤ D` between sites exhibits `(C, J)` as a dense subsite of `(D, K)` if it is cover-dense (covering sieves factor through images), locally fully faithful, and preserves/reflects covers. The main result is the comparison lemma: such functors induce an equivalence between categories of sheaves on the two sites, allowing sheaf theory on a large site to be studied via a smaller, denser subsite.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of cover-dense functors: definition of `IsCoverDense` (covering sieves factor through functor images), presheaf gluing via `pushforwardFamily`, natural transformations and isomorphisms between sheaves induced by cover-dense locally-full functors, and the `IsDenseSubsite` class combining cover-density with local full-faithfulness and cover-preservation/reflection |
| InducedTopology.lean | Induced Grothendieck topology on the domain: defines `LocallyCoverDense` functors and constructs `inducedTopology` where sieves are covers iff their pushforward is, proves the induced topology makes the functor both cover-lifting and cover-preserving, and establishes that cover-dense functors induce equivalences of sheaf categories (comparison lemma) |
| SheafEquiv.lean | Equivalence of sheaf categories for dense subsites: proves the adjunction counit is an isomorphism using the Yoneda embedding and limits over structured arrow categories, constructs the equivalence `Sheaf J A ≌ Sheaf K A` for dense subsites, and establishes compatibility with sheafification functors |

## Subdirectories

*(none)*

## Search Tags

dense-subsite cover-dense comparison-lemma grothendieck-topology sheaf-equivalence locally-full locally-faithful induced-topology cover-lifting cover-preserving functor-pushforward functor-pullback structured-arrow kan-extension sheafification-compatibility
