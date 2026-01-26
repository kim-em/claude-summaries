---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/RelIso
generated: 2026-01-26T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# RelIso

## Overview

This directory contains the core theory of relation homomorphisms, embeddings, and isomorphisms. It defines three fundamental structure-preserving maps between relations: `RelHom` (functions preserving relatedness one direction), `RelEmbedding` (injective functions preserving relatedness both directions), and `RelIso` (bijective functions preserving relatedness both directions). These are the relational analogues of function, embedding, and equivalence, and form the foundation for order-preserving maps, initial segments, and order isomorphisms used throughout the Order theory hierarchy.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of RelHom (`→r`), RelEmbedding (`↪r`), and RelIso (`≃r`); includes composition, identity, swap (dual), constructors (ofMapRelIff, ofMonotone, ofSurjective), and instances showing preservation of order properties (irreflexivity, transitivity, well-foundedness, etc.); also defines Sum.Lex and Prod.Lex embeddings/isomorphisms (sumLexCongr, prodLexCongr), quotient embeddings, and casting between relations |
| Set.lean | Interactions between relation morphisms and sets: defines Subrel (inherited relation on subtypes), Subrel.relEmbedding, Set.inclusion as relation embedding, directed/DirectedOn preservation, RelIso range theorems, codomain restriction (codRestrict), image/preimage lemmas, and well-foundedness characterization via downward intervals |

## Subdirectories

(none)

## Search Tags

relation-homomorphism relation-embedding relation-isomorphism RelHom RelEmbedding RelIso order-preserving structure-preserving monotone preimage subrelation inherited-relation well-founded-preservation quotient-embedding lexicographic sum-lex prod-lex Galois-connection directed subtype codomain-restriction initial-segment
