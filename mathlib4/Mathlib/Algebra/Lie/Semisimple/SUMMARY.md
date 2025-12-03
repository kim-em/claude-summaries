---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Lie/Semisimple
generated: 2025-12-02T00:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Semisimple

## Overview

The `Semisimple/` directory contains the theory of simple and semisimple Lie algebras, central to the Cartan-Dynkin-Killing classification. It defines irreducible Lie modules, simple Lie algebras (irreducible under adjoint action with non-abelian condition), semisimple Lie algebras (direct sums of non-abelian atomic ideals), and reductive Lie algebras (those with trivial or central radical). Major results include proving that semisimple algebras have trivial radical, that their ideal lattice forms a Boolean algebra (hence every ideal decomposes uniquely into simple ideals), equivalence of trivial radical with absence of solvable/abelian ideals, and representation-theoretic criteria: finite-dimensional algebras with irreducible faithful finite-dimensional representations are reductive, and are semisimple if the representation is trace-free. Authored primarily by Oliver Nash with contributions from Johan Commelin.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `LieModule.IsIrreducible` (simple order on Lie submodules), `LieAlgebra.HasTrivialRadical` (radical equals `⊥`), `HasCentralRadical` (radical equals center, for reductive algebras), `IsSimple` (all ideals `⊥` or `⊤` with non-abelian condition), `IsSemisimple` (supremum of atoms equals `⊤` with independence and non-abelian atoms) |
| Basic.lean | Fundamental results on simple/semisimple algebras: `IsSimple.instHasTrivialRadical`, `IsSimple.instIsSemisimple`, `IsSemisimple.isSimple_of_isAtom`, `IsSemisimple.instBooleanAlgebra` (ideal lattice is Boolean algebra via finitely atomistic construction), `IsSemisimple.instHasTrivialRadical`, equivalences `hasTrivialRadical_iff_no_solvable_ideals` and `hasTrivialRadical_iff_no_abelian_ideals`, `abelian_radical_iff_solvable_is_abelian` for Noetherian algebras |
| Lemmas.lean | Representation-theoretic characterizations: `hasCentralRadical_and_of_isIrreducible_of_isFaithful` (finite-dimensional algebra with irreducible faithful finite-dimensional triangularizable representation over characteristic zero is reductive, with center characterized by scalar actions), `hasTrivialRadical_of_isIrreducible_of_isFaithful` (additionally requiring trace-free representation gives semisimple), `trace_toEnd_eq_zero` (trace vanishing on Lie span) |

## Subdirectories

None.

## Search Tags

semisimple simple irreducible reductive radical killing-classification cartan-dynkin boolean-algebra atomistic ideal faithful-representation trace-free lie-algebra lie-module non-abelian solvable characteristic-zero triangularizable weight-space
