---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/IntermediateField/Adjoin
generated: 2026-01-24T23:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Adjoin

## Overview

The `Adjoin/` directory provides the theory of adjoining elements to fields, forming simple and finitely generated field extensions. Given a field extension `E / F` and a set `S ⊆ E`, `adjoin F S` is the smallest intermediate field containing `S`. This differs from the ring-theoretic `Algebra.adjoin` because field adjunction automatically includes inverses. The directory covers three main areas: basic definitions and lattice structure (`Defs.lean`), the relationship between `IntermediateField.adjoin` and `Algebra.adjoin` (`Algebra.lean`), and advanced results on power bases, finite generation, and composite extensions (`Basic.lean`).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `adjoin F S` adjoins a set to a field, `F⟮α⟯` notation for simple extensions; provides `CompleteLattice` instance on intermediate fields via Galois insertion with adjoin/coe; `gc` and `gi` Galois connection/insertion; `⊥`/`⊤` definitions and characterizations; `botEquiv`/`topEquiv` isomorphisms; `restrictScalars` and lattice operations (`sup`, `inf`, `sSup`, `sInf`, `iSup`, `iInf`) with their behavior on subfields/subalgebras; `AdjoinSimple.gen` for the generator of `F⟮α⟯`; `FG` predicate for finitely generated intermediate fields; induction principles `induction_on_adjoin_finset` and `induction_on_adjoin_fg`; `map`/`comap` behavior with adjoin; `extendScalars` lemmas |
| Basic.lean | Advanced adjoin results: `mem_adjoin_simple_iff` characterizes `x ∈ F⟮α⟯` via rational functions; `finiteDimensional_sup` shows compositum of finite extensions is finite; `adjoin_rank_le_of_isAlgebraic` bounds rank of adjunction; `adjoin_simple_isCompactElement` proves simple extensions are compact in the lattice; `IsCompactlyGenerated` instance for intermediate fields; `exists_finset_of_mem_iSup` extracts finite witnesses from suprema; `adjoinRootEquivAdjoin` gives `AdjoinRoot (minpoly F α) ≃ₐ[F] F⟮α⟯`; `adjoin.powerBasis` constructs power basis for simple extensions; `adjoin.finrank` shows `[F⟮α⟯ : F] = deg(minpoly F α)`; `algHomAdjoinIntegralEquiv` bijects `F⟮α⟯ →ₐ[F] K` with roots of minimal polynomial; `minpoly.algEquiv` gives canonical isomorphism between `F⟮x⟯` and `F⟮y⟯` when `x, y` have same minimal polynomial; `Polynomial.irreducible_comp` criterion for irreducibility of composed polynomials |
| Algebra.lean | Relationship between `IntermediateField.adjoin` and `Algebra.adjoin`: `algebra_adjoin_le_adjoin` shows `Algebra.adjoin F S ≤ adjoin F S`; `adjoin_eq_algebra_adjoin` gives equality when algebra adjoin is closed under inverses; `IsFractionRing` instance showing `adjoin F S` is the fraction field of `Algebra.adjoin F S`; `fg_top_iff` relates `FG` to `Algebra.EssFiniteType`; `adjoin_toSubalgebra_of_isAlgebraic` shows `adjoin F S = Algebra.adjoin F S` for algebraic sets; `sup_toSubalgebra_of_isAlgebraic` relates compositum to subalgebra sup when one factor is algebraic; `finite_of_fg_of_isAlgebraic` shows finitely generated algebraic extensions are finite; `IsFractionRing.liftAlgHom_fieldRange` characterizes images of lifted algebra homs |

## Subdirectories

(none)

## Search Tags

adjoin intermediate-field field-extension simple-extension finitely-generated power-basis adjoin-root galois-insertion lattice-structure compositum algebra-adjoin fraction-ring minimal-polynomial algebraic finite-dimensional irreducibility
