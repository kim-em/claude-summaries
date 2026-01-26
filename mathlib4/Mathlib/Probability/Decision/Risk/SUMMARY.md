---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Decision/Risk
generated: 2026-01-26T20:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Risk

## Overview

The `Risk/` directory formalizes the theory of risk for statistical estimators in decision-theoretic frameworks. It provides definitions and theorems for analyzing the performance of estimators that map observed data to estimates of unknown parameters. The core concepts include average risk (expected loss under a prior distribution), Bayes risk (optimal expected loss achievable by any estimator), and minimax risk (worst-case optimal loss). The directory contains fundamental inequalities relating these risk measures and data-processing theorems showing how information loss increases risk.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of avgRisk, bayesRisk, and minimaxRisk with basic properties for zero/empty cases |
| Basic.lean | Fundamental inequalities (Bayes risk ≤ minimax risk), data-processing inequalities, boundedness results, and analysis of information-free scenarios |

## Subdirectories

(No subdirectories)

## Search Tags

risk-theory estimators average-risk bayes-risk minimax-risk loss-function statistical-estimation decision-theory data-processing-inequality markov-kernels measure-theory probability-theory information-theory const-kernel subsingleton-observations bounded-loss
