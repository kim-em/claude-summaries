---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Integrals
generated: 2025-12-05T00:00:00Z
git_sha: 9f4e7a48e4c91404feac52c10298674a9361184f
git_branch: HEAD
status: complete
files_count: 3
subdirs_count: 0
---

# Integrals

## Overview

The `Integrals/` directory provides explicit evaluations of definite integrals for special functions. It contains closed-form formulas for interval integrals of elementary functions (polynomials, exponentials, logarithms, trigonometric functions) and special integrals involving combinations of these. The main file `Basic.lean` serves as a comprehensive collection that enables automated integral computation via `simp` or `norm_num` for common cases. Additional files handle specialized evaluations: logarithms of trigonometric functions (computing special values of dilogarithms) and harmonic analysis results connecting circle averages to logarithmic functions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Comprehensive collection of 619 lines proving explicit interval integral formulas for elementary functions; includes change of variables lemmas, integrals of powers (x^n, x^r, complex powers), exponentials, logarithms, inverse functions, trigonometric functions (sin, cos and their powers), and reduction formulae for sin^n and cos^n used in Wallis product for π |
| LogTrigonometric.lean | Evaluates integrals of log(sin x) over [0, π/2] and [0, π]; proves ∫₀^(π/2) log(sin x) dx = -log(2)·π/2 and ∫₀^π log(sin x) dx = -log(2)·π, providing special values of the dilogarithm function Li₂ |
| PosLogEqCircleAverage.lean | Represents log⁺ (positive part of logarithm) as a circle average; proves circleAverage(log ‖· - a‖) over the unit circle equals log⁺ ‖a‖; uses harmonic function theory and connects logarithmic integrals to mean value properties |

## Subdirectories

*(None - this is a leaf folder)*

## Search Tags

interval-integrals special-functions elementary-functions power-integrals exponential-integrals logarithmic-integrals trigonometric-integrals sin-cos-integrals reduction-formulae wallis-product dilogarithm li2 log-sin circle-average harmonic-functions mean-value change-of-variables integration-by-parts closed-form-formulas definite-integrals simp-lemmas
