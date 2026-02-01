---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/SimpleModule
generated: 2026-02-01T21:00:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 6
subdirs_count: 0
---

# SimpleModule

## Overview

The `SimpleModule/` directory formalizes the theory of simple and semisimple modules in ring theory. Simple modules are those with no proper submodules (only ⊥ and ⊤), while semisimple modules are direct sums of simple modules (equivalently, every submodule has a complement). The directory includes fundamental results like Schur's Lemma (endomorphism ring of a simple module is a division ring), the Wedderburn–Artin theorem (classifying simple Artinian rings as matrix algebras over division rings), and the theory of isotypic components (decomposition of semisimple modules by isomorphism type of simple constituents).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and results: IsSimpleModule, IsSemisimpleModule, IsSemisimpleRing classes; Schur's Lemma (division ring structure on endomorphisms); characterizations of semisimple modules; simple modules as quotients by maximal ideals; products and quotients of semisimple rings |
| WedderburnArtin.lean | Wedderburn–Artin theorem: simple Artinian rings are isomorphic to matrix algebras over division rings; semisimple algebras decompose as finite products of matrix algebras; characterization of simple rings via Artinian property and minimal left ideals |
| Isotypic.lean | Isotypic modules (all simple submodules mutually isomorphic) and isotypic components; fully invariant submodules; decomposition of semisimple modules into isotypic components; endomorphism ring decompositions for direct sums of fully invariant submodules |
| InjectiveProjective.lean | Modules over semisimple rings are both injective and projective (extension and lifting properties) |
| IsAlgClosed.lean | Wedderburn–Artin theorem over algebraically closed fields: finite-dimensional simple algebras are matrix algebras over the field; finite-dimensional semisimple algebras are products of matrix algebras |
| Rank.lean | Module over a division ring is simple iff it has rank (finrank) one |

## Subdirectories

(none)

## Search Tags

simple-module semisimple-module semisimple-ring Schur-lemma endomorphism-ring division-ring Wedderburn-Artin-theorem Artinian-ring matrix-algebra isotypic-component fully-invariant-submodule maximal-ideal minimal-ideal injective-module projective-module algebraically-closed-field finite-dimensional division-algebra finrank composition-series
