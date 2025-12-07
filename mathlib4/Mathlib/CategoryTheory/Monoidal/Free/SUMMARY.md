---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Free
generated: 2025-12-07T21:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Free

## Overview

The `Free/` directory implements the free monoidal category construction and proves the monoidal coherence theorem. Given any type `C`, it constructs `FreeMonoidalCategory C` whose objects are formal tensor product expressions and whose morphisms are compositions and tensor products of structural isomorphisms (associators and unitors). The coherence theorem is proved by showing this category is thin (at most one morphism between any two objects), establishing that all diagrams built from monoidal structure commute.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Construction of free monoidal category with inductive objects (unit, tensor, of), formal morphisms (Hom), quotient by monoidal relations (HomEquiv), and universal property via projection functor to any monoidal category |
| Coherence.lean | Proof of monoidal coherence theorem by defining normal forms (left-associated expressions), normalization functor to discrete category of normal objects, natural isomorphism between identity and normalization, proving the free monoidal category is thin and a groupoid |

## Subdirectories

None.

## Search Tags

free-monoidal-category monoidal-coherence-theorem normal-forms thin-category groupoid formal-tensor-products associators unitors universal-property quotient-category normalization categorical-coherence
