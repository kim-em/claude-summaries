---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Notation
generated: 2025-12-01T20:15:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 7
subdirs_count: 1
---

# Notation

## Overview

The `Notation/` directory contains definitions and minimal theory for basic algebraic notation, positioned at the very bottom of the algebraic hierarchy. It defines the fundamental notation typeclasses for algebraic operators (`0`, `1`, `+`, `-`, `*`, `/`, `+ᵥ`, `•`, `-ᵥ`) and establishes critical function-level algebraic infrastructure. This folder is deliberately kept import-minimal and forbidden from importing anything outside `Algebra/Notation` to ensure it remains early in the import hierarchy. Key concepts span three layers: (1) notation typeclasses (`HVAdd`, `VAdd`, `VSub`, `Star`) for operators, (2) function support theory (the set where a function is non-zero/non-one) and indicator functions for restricting functions to sets, and (3) pointwise algebraic operations on product types and Pi types. The Pi/ subdirectory extends this foundation to dependent function types, establishing how algebraic operators apply componentwise and introducing the crucial `mulSingle`/`single` construction for functions supported at a single index.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Documents that this folder contains basic algebraic notation and must stay extremely early in the import hierarchy |
| Defs.lean | Defines core notation typeclasses: `HVAdd`/`VAdd` (additive actions `+ᵥ`), `VSub` (difference `-ᵥ`), `Star` (star operation without default notation), and interaction lemmas for `if-then-else` with multiplication/division |
| Lemmas.lean | Inequality lemmas involving `1` and `0` with conditional expressions (`dite`/`ite`), providing comparison infrastructure before full group theory |
| Support.lean | Defines `mulSupport f = {x \| f x ≠ 1}` and `support f = {x \| f x ≠ 0}` with comprehensive lemmas for set operations, function updates, extensions, and products |
| Indicator.lean | Defines `mulIndicator s f a = if a ∈ s then f a else 1` (and additive variant) with properties for composition, preimage, and relationships to function support |
| Prod.lean | Componentwise notation for arithmetic on product types `M × N`: instances for `One`, `Mul`, `Inv`, `Div`, `SMul`, `Pow`, `Star` without full algebraic structure |
| FiniteSupport.lean | Proves finiteness of function support along fibers for product-domain functions |

## Subdirectories

- [x] `Pi/` - Pointwise algebraic notation and operations for dependent function types; defines `mulSingle`/`single` for single-index-supported functions

## Search Tags

notation typeclass algebraic-operators scalar-multiplication vector-addition support indicator-function prod-instances star-operation import-hierarchy hvad vadd vsub smul
