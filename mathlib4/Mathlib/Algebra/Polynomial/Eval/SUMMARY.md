---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Polynomial/Eval
generated: 2025-12-01T10:32:45Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 7
subdirs_count: 0
---

# Eval

## Overview

The `Eval/` directory contains comprehensive theory for polynomial evaluation, implementing `eval₂` (evaluation with ring homomorphism), `eval` (evaluation in the same ring), `comp` (polynomial composition), and `map` (coefficient mapping). These fundamental operations connect polynomials to their values, enabling evaluation at points, mapping between rings, and composing polynomials. The directory covers interactions with degree theory, coefficient structure, algebra homomorphisms, irreducibility preservation, and scalar multiplication.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core evaluation definitions: `eval₂ f x` evaluates polynomial applying ring hom `f` to coefficients and substituting `x` for variable; `eval x` evaluates at `x`; `IsRoot p a` tests if `a` is a root; `comp p q` composes polynomials; `map f` applies `f` to coefficients. Includes bundled versions as ring homomorphisms and extensive API for `C`, `X`, arithmetic operations |
| Algebra.lean | Evaluation in algebras: specialized lemmas for `eval₂` when the ring homomorphism is `algebraMap R S`, proving multiplication/power/composition properties in algebra contexts |
| Coeff.lean | Interaction of evaluation with coefficients: `coeff_map` shows `(p.map f).coeff n = f (p.coeff n)`; `eval₂_C_X` identity; `coeff_zero_eq_eval_zero`; map injectivity/surjectivity; `piEquiv` isomorphism for product rings; evaluation at zero/one/nat/int casts |
| Degree.lean | Interaction of evaluation with degrees: `eval₂_eq_sum_range` expresses evaluation as sum over degree range; `comp` degree formulas; `map` degree bounds (`degree_map_le`, `natDegree_map_of_leadingCoeff_ne_zero`); `mapEquiv` ring equivalence; `iterate_comp_eval` for iterated composition |
| Irreducible.lean | Irreducibility preservation under mapping: `Monic.irreducible_of_irreducible_map` proves monic polynomial irreducible in `R` if its image under `φ : R →+* S` is irreducible in `S` (crucial for proving irreducibility over `ℤ` via reduction modulo primes) |
| SMul.lean | Scalar multiplication interaction: `eval₂_smul`, `eval_smul`, `map_smul`, `comp_smul` show these operations preserve scalar multiplication; `leval` provides `eval` as a linear map |
| Subring.lean | Subring characterization: `mem_map_rangeS` and `mem_map_range` characterize polynomials in the range of `mapRingHom f` as exactly those with coefficients in the range of `f` |

## Subdirectories

None.

## Search Tags

polynomial evaluation eval eval₂ aeval ring-homomorphism polynomial-composition polynomial-map isroot coefficients degree irreducible monic scalar-multiplication linear-map subring algebra-homomorphism
