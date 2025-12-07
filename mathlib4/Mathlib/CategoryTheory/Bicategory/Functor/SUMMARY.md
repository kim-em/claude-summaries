---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory/Functor
generated: 2025-12-07T21:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 9
subdirs_count: 0
---

# Functor

## Overview

The `Functor/` directory formalizes the hierarchy of functors between bicategories. Unlike ordinary category theory where functors strictly preserve composition and identities, bicategorical functors must account for the weak coherence structure of bicategories. This directory implements the full spectrum from prelax functors (minimal structure, preserving only 2-morphism composition) through lax and oplax functors (with coherent natural transformations `mapId` and `mapComp`) to pseudofunctors (where these natural transformations are invertible) and finally strict pseudofunctors (where composition and identities are preserved on the nose). The files establish the foundational infrastructure for working with bicategorical functors, including specialized constructors for locally discrete bicategories and the bicategory Cat of categories.

## Key Files

| File | Purpose |
|------|---------|
| Prelax.lean | Prelax functors: basic structure with map on objects, 1-morphisms, and 2-morphisms preserving composition |
| Lax.lean | Lax functors: prelax functors with coherent 2-morphisms mapId and mapComp (composition up to 2-morphism) |
| Oplax.lean | Oplax functors: dual notion to lax functors with reversed 2-morphisms for mapId and mapComp |
| Pseudofunctor.lean | Pseudofunctors: oplax/lax functors where mapId and mapComp are isomorphisms (composition up to coherent isomorphism) |
| StrictlyUnitary.lean | Strictly unitary lax functors and pseudofunctors where mapId is identity (map preserves identity 1-morphisms strictly) |
| StrictPseudofunctor.lean | Strict pseudofunctors: strictly unitary pseudofunctors where both mapId and mapComp are given by eqToIso |
| LocallyDiscrete.lean | Specialized constructors for pseudofunctors and oplax functors from locally discrete bicategories where all 2-morphisms are identities |
| Cat.lean | Naturality properties of mapId' and mapComp' for pseudofunctors to the bicategory Cat of categories |
| Strict.lean | Deprecated module redirecting to Mathlib.CategoryTheory.Bicategory.Strict.Pseudofunctor (deprecated since 2025-10-02) |

## Subdirectories

(No subdirectories)

## Search Tags

bicategory functor prelax-functor lax-functor oplax-functor pseudofunctor strict-pseudofunctor strictly-unitary normal-homomorphism 2-functor weak-functor homomorphism mapId mapComp map₂ whiskering coherence locally-discrete cat functoriality
