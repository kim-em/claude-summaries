---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Polynomial/Degree
generated: 2025-12-01T10:43:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 11
subdirs_count: 0
---

# Degree

## Overview

The `Degree/` folder contains comprehensive theory for polynomial degrees over semirings and rings, including core definitions (`degree`, `natDegree`, `leadingCoeff`, `Monic`), extensive lemmas for degree calculations under operations (multiplication, addition, composition), trailing degree theory (lowest exponent), support/coefficient relationships, domain properties (no zero divisors), unit characterizations, and specialized results for small-degree polynomials and finite fields (absolute value via `cardPowDegree`).

## Key Files

| File | Purpose |
|------|---------|
| Definitions.lean | Core definitions: `degree p` (highest exponent as `WithBot ℕ`, `⊥` for zero polynomial), `natDegree p` (degree as `ℕ`, 0 for zero), `leadingCoeff p` (coefficient at `natDegree`), `Monic p` (leading coefficient is 1), and fundamental theorems relating degree/natDegree |
| Lemmas.lean | Core degree lemmas: `natDegree_comp_le` (composition degree bound), `degree_pos_of_root`, coefficient/degree relationships, leading coefficient behavior under addition by degree comparison, well-foundedness of degree ordering |
| Operations.lean | Degree behavior under polynomial operations: addition, multiplication, scalar multiplication, powers, negation, subtraction (31KB comprehensive theory) |
| TrailingDegree.lean | Trailing degree theory: `trailingDegree p` (lowest exponent as `ℕ∞`, `⊤` for zero), `natTrailingDegree`, `trailingCoeff`, `TrailingMonic` (trailing coefficient is 1), mirroring the leading degree API for the bottom end of polynomials |
| Domain.lean | Degree theory in domains (no zero divisors): exact degree formulas for multiplication/powers (`natDegree_mul`, `natDegree_pow`), divisibility/degree relationships, integral domain lemmas |
| Units.lean | Unit polynomial characterization: degree zero conditions for units, `isUnit_iff` (unit iff constant polynomial `C r` with unit `r`), monic divisibility properties |
| SmallDegree.lean | Results for specific small degrees: characterizing degree ≤ 1 polynomials as `C a * X + C b`, monic linear polynomials as `X + C b`, degree bounds for linear polynomials |
| Support.lean | Relationship between polynomial support and degree: `natDegree_mem_support_of_nonzero`, expressing polynomials as sums over support or ranges, support subset of `range (natDegree + 1)` |
| Monomial.lean | Degree theory for monomials: lemmas for `natDegree_le_pred`, reconstructing polynomials from leading coefficient and natDegree for singleton-support polynomials |
| IsMonicOfDegree.lean | Structure and API for monic polynomials of given degree: `IsMonicOfDegree p n` combines `p.natDegree = n` and `p.Monic`, closure under multiplication, decomposition lemmas |
| CardPowDegree.lean | Absolute value on polynomials over finite fields: `cardPowDegree` maps `p` to `q^(degree p)` for finite field of cardinality `q`, proving it respects Euclidean domain structure |

## Subdirectories

*(None)*

## Search Tags

polynomial degree natDegree leadingCoeff monic trailing-degree support semiring ring domain no-zero-divisors composition multiplication addition units finite-field absolute-value euclidean-domain well-founded small-degree linear-polynomial
