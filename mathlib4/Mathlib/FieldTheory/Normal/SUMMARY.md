---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/Normal
generated: 2026-01-24T22:40:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Normal

## Overview

The `Normal/` directory formalizes normal field extensions, which are algebraic extensions where every element's minimal polynomial splits completely. It provides the core definition (`Normal F K` typeclass), proves the equivalence between being normal and being a splitting field for finite extensions, develops the theory of restricting and lifting algebra homomorphisms through normal subfields, and constructs normal closures of field extensions with their associated uniqueness theorems.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Normal F K` typeclass (minimal polynomials split), basic properties, tower results (`Normal.tower_top_of_normal`), restriction of algebra homomorphisms to normal subfields (`AlgHom.restrictNormal`), group homomorphism structure (`AlgEquiv.restrictNormalHom`), and the equivalence between F-algebra homomorphisms and automorphisms for normal extensions |
| Basic.lean | Proves equivalence between being normal and being a splitting field (`Normal.of_isSplittingField`, `Normal.exists_isSplittingField`), compositum and intersection results (normal extensions are closed under sups, infs, iSup, iInf), lifting of algebra homomorphisms to larger normal extensions (`AlgHom.liftNormal`), surjectivity of restriction maps, solvability inheritance through towers, and Galois conjugacy results (roots of the same minimal polynomial are in the same orbit) |
| Closure.lean | Normal closure construction: `IntermediateField.normalClosure F K L` as the supremum of all F-algebra embeddings of K into L, the `IsNormalClosure` predicate characterizing when a field is the normal closure, uniqueness theorem (`IsNormalClosure.equiv`), closure operator properties (monotone, idempotent), characterizations of normality via invariance under embeddings and automorphisms, and cardinality results for algebra homomorphisms when minimal polynomials split |

## Subdirectories

(none)

## Search Tags

normal-extensions normal-closure field-theory splitting-field minimal-polynomial algebra-homomorphisms galois-conjugates tower-extensions intermediate-fields field-embeddings automorphism-groups restriction-lift closure-operator algebraic-extensions
