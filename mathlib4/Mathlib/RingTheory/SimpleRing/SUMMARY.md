---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/SimpleRing
generated: 2026-02-01T22:30:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 6
subdirs_count: 0
---

# SimpleRing

## Overview

The `SimpleRing/` directory contains the theory of simple rings - rings with only two two-sided ideals (⊥ and ⊤). This includes the core definition, basic properties (nontriviality, injectivity of ring homomorphisms from simple rings), preservation under surjective homomorphisms and isomorphisms, connections to fields (center of a simple ring is a field, commutative simple rings are fields), and specialized results for matrix rings and principal ideal domains.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `IsSimpleRing` as a predicate expressing that the lattice of two-sided ideals is simple (only ⊥ and ⊤) |
| Basic.lean | Fundamental properties: simple rings are nontrivial, division rings are simple, ring homomorphisms from simple rings to nontrivial rings are injective, characterization via injective homomorphisms, simplicity of opposite rings |
| Congr.lean | Preservation of simplicity: surjective ring homomorphisms and ring isomorphisms preserve simplicity; characterization via two-sided one-sided ideals for commutative rings |
| Field.lean | Connection to fields: the center of a simple ring is a field (`isField_center`), commutative simple rings are exactly fields (`isSimpleRing_iff_isField`) |
| Matrix.lean | Matrix ring instance: the matrix ring `Matrix ι ι A` over a simple ring `A` is simple (requires finite nonempty index type) |
| Principal.lean | Principal ideal domain instance: commutative simple rings are principal ideal domains (and integral domains) since they are fields |

## Subdirectories

*(No subdirectories)*

## Search Tags

simple-ring two-sided-ideal division-ring field center matrix-ring principal-ideal-domain ring-homomorphism injectivity isomorphism lattice-theory commutative-ring
