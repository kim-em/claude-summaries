---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Functor
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Functor

## Overview

The `Functor/` subdirectory provides a bridge between programming-style applicative functors (as used in Lean's `Type`-based functional programming) and category theory's lax monoidal functors. It defines how a lawful applicative functor on types can be viewed as a lax monoidal functor between the monoidal category of types, enabling the use of applicative functors from Lean's standard library within categorical constructions.

## Key Files

| File | Purpose |
|------|---------|
| Types.lean | Converts lawful `Applicative` functors to `LaxMonoidal` functors with unit morphism `ε` mapping to `pure PUnit.unit` and tensor morphism `μ` using applicative application `<*>` |

## Subdirectories

(None)

## Search Tags

monoidal-functors lax-monoidal applicative-functors type-functors category-theory-programming-bridge lawful-applicative functor-categories types
