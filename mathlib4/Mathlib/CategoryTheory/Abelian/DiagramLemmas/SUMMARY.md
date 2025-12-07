---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian/DiagramLemmas
generated: 2025-12-07T15:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# DiagramLemmas

## Overview

The `DiagramLemmas/` directory contains fundamental diagram-chasing lemmas for abelian categories, including the classic four lemma, five lemma, and snake lemma. These results are essential tools for proving properties about exact sequences and commutative diagrams. The four lemma establishes monomorphism or epimorphism properties of middle vertical maps in commutative diagrams with exact rows, while the five lemma (deduced from the four lemma) shows that the middle map is an isomorphism when the surrounding four maps are. The snake lemma constructs long exact sequences relating kernels and cokernels of composable morphisms.

## Key Files

| File | Purpose |
|------|---------|
| Four.lean | Four and five lemmas for commutative diagrams with exact rows in abelian categories; proves middle map is mono/epi/iso based on properties of surrounding maps in diagrams on `ComposableArrows C n`; includes specialized three lemma variants for shorter sequences and convenience API for `ShortComplex` |
| KernelCokernelComp.lean | Snake lemma application constructing the long exact sequence `0 → ker f → ker (f ≫ g) → ker g → coker f → coker (f ≫ g) → coker g → 0` for composable morphisms; proves exactness via snake input built from split exact sequences of binary biproducts |

## Subdirectories

(none)

## Search Tags

diagram-lemmas four-lemma five-lemma snake-lemma exact-sequences diagram-chasing abelian-categories commutative-diagrams kernel-cokernel-sequences homological-algebra long-exact-sequences
