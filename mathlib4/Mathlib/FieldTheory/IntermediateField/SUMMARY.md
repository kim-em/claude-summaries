---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/IntermediateField
generated: 2026-01-24T23:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 1
---

# IntermediateField

## Overview

The `IntermediateField/` directory provides the foundational theory of intermediate fields in field extensions. Given a field extension `L / K`, an intermediate field is a subfield of `L` containing the image of `K`, forming a tower `L / S / K`. This infrastructure is essential for Galois theory, as intermediate fields correspond to subgroups of the Galois group. The directory covers the basic structure theory, algebraic properties of intermediate fields, and the theory of adjoining elements to create simple and finitely generated extensions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `IntermediateField K L` as a structure extending `Subalgebra K L` with inverse closure; provides SetLike instance, field structure on intermediate fields, coercion lemmas, map/comap operations along AlgHoms, scalar tower instances, `restrictScalars` for viewing intermediate fields over smaller base fields, `lift` for lifting intermediate fields through towers, and `extendScalars` order isomorphisms |
| Algebraic.lean | Results connecting intermediate fields with algebraicity and finite dimensionality; proves `FiniteDimensional K F` for intermediate fields when `L/K` is finite-dimensional; provides `eq_of_le_of_finrank_le` for comparing intermediate fields by dimension; shows algebraic subalgebras are intermediate fields via `Subalgebra.IsAlgebraic.toIntermediateField`; establishes `subalgebraEquivIntermediateField` order isomorphism when `L/K` is algebraic |

## Subdirectories

- [ ] `Adjoin/` - Theory of adjoining elements to fields: definitions of `adjoin F S` and `F⟮α⟯` notation, lattice structure on intermediate fields, Galois connection with `Algebra.adjoin`, power bases for simple extensions, finitely generated extensions, results on compositum of fields

## Search Tags

intermediate-field field-extension subalgebra subfield algebra-tower restrict-scalars extend-scalars finite-dimensional algebraic galois-theory field-tower adjoin simple-extension
