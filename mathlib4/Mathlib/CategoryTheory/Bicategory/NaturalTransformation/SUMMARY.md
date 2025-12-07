---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory/NaturalTransformation
generated: 2025-12-07T08:22:55Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# NaturalTransformation

## Overview

This directory formalizes natural transformations between various kinds of functors in bicategory theory. Unlike ordinary category theory where natural transformations require equality in the naturality square, bicategorical natural transformations use specified 2-morphisms (or 2-isomorphisms) instead. The directory provides three variants (lax, oplax, and strong transformations) for both lax functors and oplax functors, plus the specialized case for pseudofunctors.

## Key Files

| File | Purpose |
|------|---------|
| Lax.lean | Lax, oplax, and strong transformations between lax functors with vertical composition and CategoryStruct instances |
| Oplax.lean | Lax, oplax, and strong transformations between oplax functors with naturality conditions and whiskering lemmas |
| Pseudo.lean | Strong transformations between pseudofunctors with conversion to/from oplax transformations and CategoryStruct instance |
| Strong.lean | Deprecated module (since 2025-05-11) that re-exports Pseudofunctor and Oplax modules |

## Subdirectories

None - this is a leaf directory.

## Search Tags

natural-transformation bicategory lax-transformation oplax-transformation strong-transformation pseudofunctor lax-functor oplax-functor vertical-composition naturality-condition 2-morphism bicategorical-naturality whiskering categoryStruct
