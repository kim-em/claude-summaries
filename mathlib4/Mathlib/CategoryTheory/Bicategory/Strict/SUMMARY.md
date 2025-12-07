---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory/Strict
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Strict

## Overview

The `Strict/` subdirectory formalizes strict bicategories (often called strict 2-categories in the literature), where the coherence isomorphisms (left unitors, right unitors, and associators) are given by equalities rather than arbitrary isomorphisms. This strictness allows the bicategory to be treated as an ordinary category. The directory also provides specialized API for pseudofunctors, lax functors, and oplax functors from strict bicategories, including compatibility lemmas for composition with identities, associativity, and commutative square diagrams.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `Bicategory.Strict` typeclass requiring unitors/associators to be `eqToIso` of actual equalities; category instance for strict bicategories; whiskering lemmas for `eqToHom` morphisms |
| Pseudofunctor.lean | API for pseudofunctors from strict bicategories including `mapComp'` compatibility with identity composition and associativity; `isoMapOfCommSq` construction for commutative squares; similar lemmas for lax and oplax functors |

## Subdirectories

*(None)*

## Search Tags

strict-bicategory strict-2-category eqToIso coherence-isomorphism unitor associator pseudofunctor lax-functor oplax-functor mapComp commutative-square whiskering category-instance
