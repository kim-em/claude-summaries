---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/NumberField/InfinitePlace
generated: 2026-01-25T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# InfinitePlace

## Overview

This directory contains the formalization of infinite places of number fields and their properties. Infinite places correspond to complex embeddings and capture the archimedean structure of number fields. The theory includes the basic definition of infinite places as equivalence classes of complex embeddings (where φ and its conjugate define the same place), classification into real and complex places with multiplicities 1 and 2 respectively, completions at infinite places yielding ℝ or ℂ, ramification theory for field extensions, and characterization of totally real and totally complex number fields.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `InfinitePlace K` as subtype of absolute values arising from complex embeddings, `IsReal` vs `IsComplex` predicates, multiplicity (1 for real, 2 for complex), product formula relating norms across infinite places to field norm, and density of diagonal embedding in product of completions |
| Completion.lean | Completion at infinite places using `AbsoluteValue.Completion`, showing completions are locally compact normed fields, with ring isomorphisms to ℝ (real places) or ℂ (complex places) via extension embeddings |
| Embeddings.lean | Embedding theory: finiteness and cardinality of embeddings equals finrank, roots of minimal polynomials are images under embeddings, Kronecker's theorem (algebraic integers with all conjugates in unit disk are roots of unity), and place construction from embeddings |
| Ramification.lean | Ramification at infinite places: `comap` operation for restriction, Galois group action on places via comap, `IsUnramified` when multiplicities match (real-to-real or complex-to-complex), `IsRamified` when complex place lies over real place, orbit structure under Galois action, and relationship to even/odd degree extensions |
| TotallyRealComplex.lean | Totally real fields (all places real, equivalently nrComplexPlaces = 0), totally complex fields (all places complex, equivalently nrRealPlaces = 0), maximal real subfield construction (largest totally real subfield containing all others), and finrank formulas for totally real/complex fields |

## Subdirectories

(none)

## Search Tags

infinite-place complex-embedding real-embedding absolute-value archimedean-place completion ramification unramified totally-real totally-complex number-field-place multiplicity conjugate-embedding galois-orbit product-formula norm-map kronecker-theorem maximal-real-subfield weak-approximation dense-embedding
