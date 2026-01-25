---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/JacobiSum
generated: 2026-01-25T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# JacobiSum

## Overview

The `JacobiSum/` directory provides a comprehensive formalization of Jacobi sums for multiplicative characters on finite commutative rings and fields. The theory generalizes the classical construction from Ireland & Rosen, defining the Jacobi sum `J(χ,ψ) = ∑ x : R, χ x * ψ (1 - x)` and establishing fundamental relations including the key formula `g(χψ) * J(χ,φ) = g(χ) * g(φ)` connecting Jacobi sums to Gauss sums. This includes special value computations, norm formulas, membership results in cyclotomic integer rings, and the power formula expressing `g(χ)^n` as a product of Jacobi sums for characters of order n.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines Jacobi sums of multiplicative characters, proves commutativity, relation to Gauss sums (`g(χψ)*J(χ,φ) = g(χ)*g(φ)`), special values (J(1,1) = #F-2, J(1,χ) = -1, J(χ,χ⁻¹) = -χ(-1)), norm formula J(χ,φ)*J(χ⁻¹,φ⁻¹) = #F, membership in ℤ[μ] for cyclotomic μ, congruence modulo (μ-1)², and power formula g(χ)^n = χ(-1)*#F*∏J(χ,χⁱ) |

## Subdirectories

(none)

## Search Tags

jacobi-sum gauss-sum multiplicative-character finite-field character-sum cyclotomic number-theory quadratic-reciprocity primitive-root algebraic-integer
