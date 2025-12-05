---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Integrability
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Integrability

## Overview

This folder establishes integrability results for special functions. `Basic.lean` provides fundamental interval integrability theorems for power functions (x^n, x^r), complex powers, trigonometric functions (sin, cos), exponential, logarithm, and related functions over real intervals. `LogMeromorphic.lean` extends these results to logarithms of meromorphic functions, proving interval integrability for `log ‖f‖` when f is real-meromorphic on compact intervals (including specific cases like log∘sin and log∘cos), and circle integrability for `log ‖f‖` when f is complex-meromorphic on circles in the complex plane.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Interval integrability for fundamental special functions: powers (x^n, x^r, x^z), logarithm, exponential, trigonometric functions, and their compositions; includes characterizations like `integrableOn_Ioo_rpow_iff` showing x^s is integrable on (0,t) iff -1 < s |
| LogMeromorphic.lean | Integrability of logarithms of meromorphic functions; proves `log ‖f‖` is interval integrable when f is real-meromorphic on compact intervals, and circle integrable when f is complex-meromorphic on circles; includes applications to trigonometric functions (log∘sin, log∘cos) |

## Subdirectories

*(No subdirectories)*

## Search Tags

integrability interval-integrable circle-integrable special-functions power-functions logarithm exponential trigonometric meromorphic log-norm measure-theory volume-measure locally-finite-measure rpow cpow complex-power improper-integrals analytic-functions
