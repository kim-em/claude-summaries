---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory/Functor
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 9
subdirs_count: 0
---

# Functor

## Overview

The `Functor/` directory contains the formalization of various notions of functors between bicategories in mathlib4. It implements a hierarchy of functor types, starting from the most flexible prelax functors (which only preserve 2-morphisms functorially) up to strict pseudofunctors (which preserve composition and identities strictly). The directory includes prelax, lax, oplax, and pseudofunctors, as well as specialized variants like strictly unitary functors and strict pseudofunctors, along with constructors for building functors from locally discrete bicategories and to the bicategory of categories (Cat).

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
