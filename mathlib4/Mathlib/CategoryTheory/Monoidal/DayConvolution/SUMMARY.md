---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/DayConvolution
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# DayConvolution

## Overview

The `DayConvolution/` directory extends the Day convolution monoidal structure on functor categories with additional categorical structures. It proves that when both source and target categories are braided/symmetric monoidal, the Day convolution preserves these structures, establishes that monoidal closed structure on the target lifts to Day convolution via internal hom functors, and provides a type synonym `DayFunctor` that equips functor categories with Day convolution as their canonical monoidal structure.

## Key Files

| File | Purpose |
|------|---------|
| Braided.lean | Braiding and symmetry for Day convolution - constructs explicit braiding isomorphism when C and V are braided, proves hexagon identities, and shows symmetry is preserved |
| Closed.lean | Internal hom functors for Day convolution in monoidal closed categories - defines `DayConvolutionInternalHom` structure with ends, constructs evaluation and coevaluation morphisms, proves triangle identities |
| DayFunctor.lean | Type synonym `DayFunctor C V` (notation `C ⊛⥤ V`) for functor categories with Day convolution monoidal structure instead of pointwise structure, provides `η` and `ν` unit transformations |

## Subdirectories

_(No subdirectories)_

## Search Tags

day-convolution braided-monoidal symmetric-monoidal monoidal-closed internal-hom functor-categories left-kan-extension hexagon-identities evaluation coevaluation ends wedges day-functor category-theory
