---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Martingale
generated: 2026-01-26T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# Martingale

## Overview

The `Martingale/` directory provides comprehensive formalization of martingale theory for discrete-time stochastic processes. It defines the core concepts of martingales, supermartingales, and submartingales with respect to filtrations, along with major convergence theorems and stopping time results. The directory includes Doob's decomposition theorem (centering lemma), the optional stopping theorem (fair game theorem), Doob's upcrossing estimate, martingale convergence theorems (both almost everywhere and L¹), the optional sampling theorem, and Lévy's generalized Borel-Cantelli lemma. These foundational results are central to modern probability theory and stochastic process analysis.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of Martingale, Supermartingale, and Submartingale; fundamental properties including strong adaptedness, integrability, conditional expectation characterizations, and set integral equalities |
| Centering.lean | Doob's decomposition theorem: any ℕ-indexed adapted integrable process can be uniquely decomposed into the sum of a martingale (martingalePart) and a predictable process (predictablePart) |
| Convergence.lean | Martingale convergence theorems: almost everywhere convergence for L¹-bounded submartingales, L¹ convergence for uniformly integrable submartingales, Lévy upwards theorems, and limit process properties |
| Upcrossing.lean | Doob's upcrossing estimate: $(b-a)\mathbb{E}[U_N(a,b)] \le \mathbb{E}[(f_N - a)^+]$ where $U_N(a,b)$ counts upcrossings from below $a$ to above $b$ before time $N$; defines upper/lower crossing times and upcrossing strategies |
| OptionalStopping.lean | Optional stopping theorem (fair game theorem): a process is a submartingale iff expected stopped values are monotone in bounded stopping times; includes Doob's maximal inequality |
| OptionalSampling.lean | Optional sampling theorem: for bounded stopping time τ and any stopping time σ, the martingale value at min(τ,σ) equals the conditional expectation of the stopped value at τ |
| BorelCantelli.lean | Lévy's generalized Borel-Cantelli lemma and one-sided martingale bound: characterizes limsup of adapted sets via conditional probabilities; defines stopped processes above thresholds (leastGE, stoppedAbove) |

## Subdirectories

*(No subdirectories)*

## Search Tags

martingale supermartingale submartingale doob-decomposition convergence-theorem optional-stopping optional-sampling upcrossing stopping-time filtration adapted-process predictable-process borel-cantelli levy-theorem maximal-inequality uniform-integrability limit-process centering-lemma fair-game-theorem
