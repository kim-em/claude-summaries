---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Module
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 12
subdirs_count: 0
---

# Module

## Overview

The `Module/` directory develops the theory of ordered modules: modules over ordered rings where scalar multiplication interacts compatibly with both the module and ring orderings. It provides fine-grained typeclasses for reasoning about monotonicity (`PosSMulMono`, `SMulPosMono`, etc.), bundled ordered module typeclasses (`IsOrderedModule`, `IsStrictOrderedModule`), order-preserving equivalences and homomorphisms, and advanced results like the Hahn embedding theorem (embedding linearly ordered modules into lexicographically ordered Hahn series) and Archimedean module theory.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of fine-grained monotonicity typeclasses for scalar multiplication: `PosSMulMono`, `PosSMulStrictMono`, `PosSMulReflectLT`, `PosSMulReflectLE` (left smul) and `SMulPosMono`, `SMulPosStrictMono`, `SMulPosReflectLT`, `SMulPosReflectLE` (right smul), plus bundled `IsOrderedModule` and `IsStrictOrderedModule` |
| Basic.lean | Further lemmas about monotonicity: relates inf/sup to scalar multiplication via absolute value (e.g., `x ⊓ y = (⅟2) • (x + y - \|y - x\|)`), proves `abs_smul` for rings, provides `PosSMulMono` positivity extension |
| OrderedSMul.lean | Deprecated `OrderedSMul` typeclass (now `IsStrictOrderedModule`) for historical compatibility with older ordered module definitions |
| Algebra.lean | Ordered algebras: proves `algebraMap` is monotone/strictly monotone when both rings are ordered compatibly, with `SMulPosMono`/`SMulPosStrictMono` instances, includes `positivity` extension |
| Field.lean | Ordered vector spaces over fields: proves `PosSMulMono → PosSMulReflectLE` and `PosSMulStrictMono → PosSMulReflectLT` for semifields, defines `OrderIso.smulRightDual` for negative scalars, includes `positivity` extension for smul |
| Rat.lean | Monotonicity of rational scalar multiplication: provides `PosSMulMono` and `PosSMulStrictMono` instances for `ℚ` and `ℚ≥0`, proves `abs_nnqsmul` and `abs_qsmul` for absolute value interaction |
| Archimedean.lean | Archimedean classes for ordered modules: proves scalar multiplication preserves Archimedean equivalence classes, defines `ArchimedeanClass.submodule`/`ball`/`closedBall` as submodules (analogous to additive subgroups) |
| HahnEmbedding.lean | **Hahn embedding theorem for ordered modules**: proves existence of strictly monotone linear map from linearly ordered module `M` over Archimedean division ring `K` to lexicographically ordered Hahn series, preserving Archimedean classes via `orderTop`, with sophisticated construction using Zorn's lemma to extend partial embeddings |
| Equiv.lean | Order type synonym equivalences: provides `toLexLinearEquiv` and `ofLexLinearEquiv` as linear equivalences for `Lex` order synonym |
| Synonym.lean | Module instances for order type synonyms: transfers module structure to `OrderDual` and `Lex` type synonyms |
| Pointwise.lean | Bounds on pointwise scalar multiplication of sets: proves `BddBelow`/`BddAbove` preservation, `lowerBounds`/`upperBounds` interaction with scalar multiplication by positive/negative scalars |
| PositiveLinearMap.lean | Positive linear maps: defines `PositiveLinearMap` structure (linear maps that are also order homomorphisms), notation `E →ₚ[R] F`, with constructor `mk₀` from nonnegative-preserving linear maps |

## Subdirectories

None.

## Search Tags

ordered-modules ordered-scalar-multiplication scalar-monotonicity module-order-interaction archimedean-modules hahn-embedding hahn-series lexicographic-order positive-linear-maps ordered-vector-spaces ordered-algebras rational-scalars order-type-synonyms pointwise-smul-bounds smul-monotonicity module-homomorphisms module-equivalences ordered-fields-modules module-archimedean-class
