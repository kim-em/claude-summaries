---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Braided
generated: 2025-12-07T10:48:50Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# Braided

## Overview

The `Braided/` directory contains the formalization of braided and symmetric monoidal categories. It implements braided monoidal categories (categories with a braiding isomorphism satisfying hexagon identities), symmetric monoidal categories (where the braiding is symmetric), braided functors (lax monoidal functors preserving the braiding), and infrastructure for transporting braided structures along equivalences. The module includes results on the Yang-Baxter equation, interactions between braiding and unitors, and Day's reflection theorem for symmetric monoidal closed categories.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of braided and symmetric monoidal categories with braiding isomorphisms, hexagon identities, Yang-Baxter equation, braided functor classes (lax, oplax, strong), and interaction between braiding and unitors |
| Multifunctor.lean | Alternative constructor for braided categories from natural isomorphisms between bifunctors, with hexagon identities phrased as natural transformations between trifunctors |
| Reflection.lean | Day's reflection theorem for symmetric monoidal closed reflective subcategories, proving equivalence of four conditions related to the reflector and showing how to lift closed monoidal structure |
| Opposite.lean | Braided category instance on opposite categories, showing that if C is braided then so is Cᵒᵖ with reversed braiding |
| Transport.lean | Infrastructure for transporting braided and symmetric monoidal structures along equivalences of categories using the Transported construction |

## Subdirectories

(none)

## Search Tags

braided-monoidal symmetric-monoidal braiding hexagon-identities yang-baxter-equation braided-functors lax-braided oplax-braided days-reflection-theorem opposite-braiding transport-braiding monoidal-categories symmetric-categories
