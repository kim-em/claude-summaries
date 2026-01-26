---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Decision
generated: 2026-01-26T21:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 0
subdirs_count: 1
---

# Decision

## Overview

The `Decision/` directory provides formalization of statistical decision theory, a framework for analyzing how estimators make decisions based on observed data. In this setting, an estimator (which may be randomized or deterministic) maps observations to estimates of unknown parameters, and the quality of these decisions is quantified by a loss function. The directory develops the fundamental theory of risk: average risk (expected loss under a prior distribution over parameters), Bayes risk (the optimal expected loss achievable by any estimator for a given prior), and minimax risk (the best worst-case loss over all possible parameter values). The formalization includes key results such as the inequality relating Bayes and minimax risk, data-processing inequalities showing how information loss increases risk, and analysis of degenerate cases where observations carry no information. This provides the mathematical foundation for comparing estimators and understanding the fundamental limits of statistical inference.

## Key Files

(No files directly in this directory)

## Subdirectories

- [x] `Risk/` - Risk theory for estimators: definitions of average risk, Bayes risk, and minimax risk, along with fundamental inequalities and data-processing theorems

## Search Tags

decision-theory statistical-decision-theory estimators risk bayes-risk minimax-risk loss-function average-risk prior-distribution data-processing-inequality estimation-theory
