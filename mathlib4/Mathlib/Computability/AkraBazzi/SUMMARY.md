---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Computability/AkraBazzi
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# AkraBazzi

## Overview

The `AkraBazzi/` subdirectory contains a complete formalization of the Akra-Bazzi theorem, a fundamental result in algorithm analysis that characterizes the asymptotic behavior of divide-and-conquer recurrences. The theorem states that for recurrences of the form `T(n) = ∑ aᵢ T(rᵢ(n)) + g(n)` where `rᵢ(n) ≈ bᵢ n`, the solution is `T(n) ∈ Θ(n^p (1 + ∑_{u=0}^{n-1} g(u) / u^{p+1}))`, where `p` is the unique real number satisfying `∑ aᵢ bᵢ^p = 1`. This implementation uses a sum-based formulation rather than the integral-based formulation found in the original theorem, as it is more directly applicable to discrete algorithmic analysis.

## Key Files

| File | Purpose |
|------|---------|
| AkraBazzi.lean | Main theorem statement and proof: defines the `AkraBazziRecurrence` structure, proves the main result `isTheta_asympBound` showing `T(n) ∈ Θ(asympBound)`, includes technical lemmas about derivatives, monotonicity, and bounds involving the smoothing function `ε(x) = 1/log x`; contains two major proof components: `T_isBigO_smoothingFn_mul_asympBound` (upper bound) and `smoothingFn_mul_asympBound_isBigO_T` (lower bound), both using strong induction on `n` |
| GrowsPolynomially.lean | Polynomial growth condition: defines `GrowsPolynomially f` predicate requiring `c₁ g(n) ≤ g(u) ≤ c₂ g(n)` for `u ∈ [b·n, n]` for any `b ∈ (0,1)`, establishes closure properties (negation, absolute value, multiplication, division, addition with little-o, powers, logarithm), proves equivalence lemmas via `IsTheta` and `IsEquivalent`, includes the key result `eventually_zero_of_frequently_zero` showing polynomially growing functions that are frequently zero must eventually be identically zero |
| SumTransform.lean | Supporting definitions and lemmas: defines `AkraBazziRecurrence` structure encoding the recurrence hypothesis, establishes existence and uniqueness of the Akra-Bazzi exponent `p` via continuity and strict anti-monotonicity of `∑ aᵢ bᵢ^p`, defines the smoothing function `ε(x) = 1/log x` with differentiability and asymptotic properties, defines `sumTransform` and `asympBound` functions, proves eventual bounds comparing sum transforms to `g(n)`, establishes positivity of `T` and asymptotic bounds along recursive branches |

## Subdirectories

None - this is a leaf directory.

## Search Tags

akra-bazzi divide-and-conquer recurrence-relations master-theorem asymptotic-analysis complexity-theory algorithm-analysis polynomial-growth sum-transform smoothing-function big-theta big-o mergesort strassen-algorithm recursion-tree induction asymptotic-bounds
