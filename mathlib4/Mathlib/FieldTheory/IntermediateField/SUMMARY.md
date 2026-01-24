---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/IntermediateField
generated: 2026-01-24T23:40:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 1
---

# IntermediateField

## Overview

The `IntermediateField/` directory provides the foundational theory of intermediate fields in field extensions. Given a field extension `L / K`, an intermediate field is a subfield of `L` containing the image of `K`, forming a tower `L / S / K`. This infrastructure is essential for Galois theory, as intermediate fields correspond to subgroups of the Galois group via the Fundamental Theorem of Galois Theory. The directory provides three main areas: basic structural theory (`Basic.lean`) defining intermediate fields as subalgebras closed under inverses with SetLike instances and map/comap operations; algebraic properties (`Algebraic.lean`) connecting intermediate fields with finite dimensionality and algebraicity; and the theory of adjoining elements (`Adjoin/` subdirectory) that constructs simple and finitely generated extensions, provides complete lattice structure, and establishes the relationship between field adjunction and ring-theoretic adjunction.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `IntermediateField K L` as a structure extending `Subalgebra K L` with inverse closure; provides SetLike instance, field structure on intermediate fields, coercion lemmas, map/comap operations along AlgHoms, scalar tower instances, `restrictScalars` for viewing intermediate fields over smaller base fields, `lift` for lifting intermediate fields through towers, and `extendScalars` order isomorphisms |
| Algebraic.lean | Results connecting intermediate fields with algebraicity and finite dimensionality; proves `FiniteDimensional K F` for intermediate fields when `L/K` is finite-dimensional; provides `eq_of_le_of_finrank_le` for comparing intermediate fields by dimension; shows algebraic subalgebras are intermediate fields via `Subalgebra.IsAlgebraic.toIntermediateField`; establishes `subalgebraEquivIntermediateField` order isomorphism when `L/K` is algebraic |

## Subdirectories

- [x] `Adjoin/` - Theory of adjoining elements to fields: core definitions (`adjoin F S`, `F⟮α⟯` notation) and complete lattice structure via Galois insertion; advanced results on power bases, minimal polynomials, and finite generation; relationship between `IntermediateField.adjoin` and `Algebra.adjoin` including fraction ring characterization

## Search Tags

intermediate-field field-extension subalgebra subfield algebra-tower restrict-scalars extend-scalars finite-dimensional algebraic galois-theory field-tower adjoin simple-extension
