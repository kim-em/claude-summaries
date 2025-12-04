---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Asymptotics
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 0
---

# Asymptotics

## Overview

The `Asymptotics/` directory contains formalization of asymptotic analysis, including big-O notation, little-o notation, and asymptotic equivalence. It provides the core definitions and theorems for comparing the growth rates of functions, including `IsBigO` (f =O[l] g), `IsLittleO` (f =o[l] g), `IsTheta` (f =Θ[l] g), and `IsEquivalent` (f ~[l] g), where `l` is a filter on the domain. These tools are essential for analyzing function behavior in limits and are used throughout analysis, particularly in calculus and complexity theory. The directory includes both general theory and specific applications to polynomial growth, exponential growth, linear growth, and superpolynomial decay.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of asymptotic relations: `IsBigOWith c l f g` (‖f‖ eventually bounded by c*‖g‖), `IsBigO` (big-O notation f =O[l] g), and `IsLittleO` (little-o notation f =o[l] g); includes basic conversions and properties |
| Lemmas.lean | Further basic lemmas about asymptotics building on the definitions; includes properties for principal filters, top filter, boundedness characterizations, and fundamental algebraic properties |
| Theta.lean | Asymptotic equivalence up to a constant: defines `IsTheta l f g` (f =Θ[l] g) as the conjunction of f =O[l] g and g =O[l] f; proves it's an equivalence relation with reflexivity, symmetry, and transitivity |
| AsymptoticEquivalent.lean | Asymptotic equivalence: defines `IsEquivalent l u v` (u ~[l] v) as (u-v) =o[l] v; proves properties including that it's an equivalence relation, characterization via tendsto for normed fields, and compatibility with arithmetic operations |
| SpecificAsymptotics.lean | Collection of specific asymptotic results for concrete functions, including power function comparisons (x^p vs x^q), polynomial division limits at infinity, and boundedness in punctured neighborhoods |
| SuperpolynomialDecay.lean | Super-polynomial decay: defines when f decays faster than any polynomial in k (all k^n * f tend to zero); proves equivalences with little-o and big-O of all powers; motivated by negligible functions in cryptography and rapidly decreasing functions in analysis |
| ExpGrowth.lean | Exponential growth of sequences u: ℕ → ℝ≥0∞ via liminf and limsup of log(u n)/n; defines `expGrowthInf` and `expGrowthSup` with properties including monotonicity and preservation of finitary Inf/Sup |
| LinearGrowth.lean | Linear growth of sequences u: ℕ → R via liminf and limsup of (u n)/n; defines `linearGrowthInf` and `linearGrowthSup`; developed primarily for R = EReal with homomorphism properties |
| TVS.lean | Generalizes big-O and little-o to topological vector spaces: defines `IsLittleOTVS` and `IsBigOTVS` using gauges instead of norms to avoid choosing canonical norms; motivated by Fréchet derivatives in topological vector spaces; proves equivalence with standard definitions in normed spaces |
| Completion.lean | Asymptotics in the completion of a normed space: proves that big-O, little-o, and theta relations are preserved under coercion to the uniform space completion (‖coe g‖ = ‖g‖ makes relations equivalent) |

## Subdirectories

None - this is a leaf directory with no subdirectories.

## Search Tags

asymptotics big-o little-o landau-notation growth-rates asymptotic-equivalence theta-notation order-notation complexity polynomial-decay exponential-growth linear-growth superpolynomial-decay topological-vector-spaces gauges completion normed-spaces filters tendsto negligible-functions
