---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Finiteness
generated: 2026-01-26T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 16
subdirs_count: 0
---

# Finiteness

## Overview

The `Finiteness/` directory provides comprehensive formalizations of various finiteness conditions in commutative algebra, focusing on finitely generated submodules, ideals, and modules. The core definitions establish `Submodule.FG` (finitely generated submodules), `Ideal.FG` (finitely generated ideals), `Module.Finite` (finite modules), and related notions including finite presentation and finite type for ring homomorphisms and algebra homomorphisms. The theory includes structural results (Nakayama's lemma, finite basis theorems), closure properties (products, quotients, sups, maps), and relationships between different finiteness notions (FG iff compact, finite iff finite-as-type for finite rings, finite presentation equivalences).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of finiteness conditions: `Submodule.FG`, `Ideal.FG`, `Module.Finite`, `RingHom.Finite`, `AlgHom.Finite` |
| Basic.lean | Basic results on finitely generated submodules including closure under sup, quotients, maps; `Module.Finite` instances and equivalences |
| Cardinality.lean | Relationships between `Module.Finite` and types with finitely many elements; existence of finite surjections from free modules; finite basis theorems |
| Nakayama.lean | Nakayama's lemma: if N is finitely generated and N ⊆ IN, then ∃r ∈ 1+I with rN = 0 |
| Ideal.lean | Finiteness properties of ideal operations: maps, compositions, radical powers, multiplication, powers |
| ModuleFinitePresentation.lean | Relations between finitely presented algebras and modules; equivalence for finite algebras (EGA IV₁ references) |
| Finsupp.lean | Finiteness results for finitely supported functions and modules |
| Bilinear.lean | Finiteness properties for bilinear maps and tensor products |
| NilpotentKer.lean | Results about nilpotent kernels in the context of finite modules |
| Nilpotent.lean | Finiteness properties involving nilpotent elements |
| Lattice.lean | Lattice structure on finitely generated submodules |
| Prod.lean | Finiteness for product modules |
| Projective.lean | Finiteness for projective modules |
| Quotient.lean | Finiteness preservation under quotients |
| Small.lean | Smallness properties (universe size) of finite modules and algebras; relates `Small.{u}` to finiteness conditions |
| Subalgebra.lean | Finiteness for subalgebras |

## Subdirectories

(No subdirectories)

## Search Tags

finiteness finitely-generated submodule ideal module finite-type finite-presentation Nakayama compact-element basis free-module quotient tensor-product bilinear nilpotent projective small universe ring-homomorphism algebra-homomorphism EGA Grothendieck commutative-algebra lattice
