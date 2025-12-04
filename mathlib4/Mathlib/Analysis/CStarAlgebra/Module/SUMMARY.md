---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/CStarAlgebra/Module
generated: 2025-12-04T14:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Module

## Overview

This directory contains the formalization of Hilbert C⋆-modules. A Hilbert C⋆-module is a complex module `E` with a right `A`-module structure (where `A` is a C⋆-algebra) and an `A`-valued inner product that satisfies the Cauchy-Schwarz inequality and induces a norm making `E` a normed vector space over `ℂ`. The theory includes the main class definition, key inequalities, constructions of specific C⋆-modules (products, pi-types, C⋆-algebras as modules over themselves, and inner product spaces), and the `WithCStarModule` type synonym for managing norm incompatibilities.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines the `CStarModule` class with `A`-valued inner product, establishes foundational properties (inner product sesquilinearity, self-adjointness, norm relations), proves the C⋆-module Cauchy-Schwarz inequality `‖⟪x, y⟫‖ ≤ ‖x‖ * ‖y‖`, and provides `normedSpaceCore` for obtaining `NormedAddCommGroup` and `NormedSpace` instances |
| Constructions.lean | Constructs `CStarModule` instances for: (1) a C⋆-algebra `A` as a module over itself with inner product `⟪x, y⟫ = y * star x`, (2) products `C⋆ᵐᵒᵈ(A, E × F)` with inner product `⟪x, y⟫ = ⟪x.1, y.1⟫ + ⟪x.2, y.2⟫`, (3) finite pi-types `C⋆ᵐᵒᵈ(A, Π i, E i)` with inner product as sum over components, and (4) inner product spaces as C⋆-modules over `ℂ`; uses bilipschitz equivalences to manage uniformity and bornology |
| Synonym.lean | Defines the `WithCStarModule A E` type synonym (notation `C⋆ᵐᵒᵈ(A, E)`) for types with a `CStarModule` structure where the C⋆-module norm differs from the existing norm; provides `equiv`, `addEquiv`, `linearEquiv`, `uniformEquiv`, and `equivL` to translate between the synonym and the original type; includes infrastructure for inheriting module structures, uniformity, and bornology; essential for products and pi-types where the C⋆-module norm doesn't match natural norms |

## Subdirectories

*(none)*

## Search Tags

hilbert-cstar-modules cstar-modules inner-product-spaces valued-inner-products normed-modules cauchy-schwarz-inequality module-constructions type-synonyms withcstarmodule products pi-types sesquilinear-maps continuous-inner-products star-modules functional-analysis operator-algebras banach-modules normed-space-core bilipschitz-equivalence
