---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Extension
generated: 2026-01-26T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 2
---

# Extension

## Overview

The `Extension/` directory formalizes the theory of algebra extensions and generators. It provides two main structures: `Algebra.Extension` represents an extension P → S of an R-algebra S (a surjective R-algebra homomorphism), and `Algebra.Generators` represents a family of generators for an algebra (an assignment of variables to values with a section of the induced polynomial map). Both structures support homomorphisms between extensions/generators, composition, base change, localization, and cotangent space constructions. The theory includes universal property characterizations and relationships between presentations and their kernels.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `Algebra.Extension` structure for extensions P → S with surjection; includes constructions (from surjective maps, trivial extension, localization, base change, infinitesimal extension); homomorphisms between extensions; cotangent space as type synonym for I/I²; cotangent module structure over S and linear maps between cotangent spaces |
| Generators.lean | Defines `Algebra.Generators` structure for families of generators (variables, values, section of R[X] → S); constructions from surjective maps, sets, algebra homomorphisms; composition, base change, extension of scalars, reindexing; homomorphisms between generators; kernel theory including decomposition for composition of generators; relationship to finite type algebras |

## Subdirectories

- [x] `Cotangent/` - Cotangent space theory for extensions
- [x] `Presentation/` - Presentations of algebras

## Search Tags

algebra-extension generators presentation polynomial-ring multivariate-polynomial surjection section cotangent-space infinitesimal-extension base-change localization composition kernel ideal finite-type scalar-tower homomorphism reindexing
