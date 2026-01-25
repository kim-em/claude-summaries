---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Zsqrtd
generated: 2026-01-25T22:15:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 4
subdirs_count: 0
---

# Zsqrtd

## Overview

The `Zsqrtd/` directory contains the formalization of integer rings of quadratic number fields ℤ[√d], where d is an integer. This includes the general theory of these rings (Basic.lean), the special case of Gaussian integers ℤ[i] = ℤ[√(-1)] with its Euclidean domain structure (GaussianInt.lean), connections to quadratic reciprocity (QuadraticReciprocity.lean), and embeddings into the real numbers (ToReal.lean). The theory establishes ring structures, norm functions, ordering when d is nonsquare, and proves key results like the classification of primes in ℤ[i] via the congruence mod 4.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and theory for ℤ√d: structure as `⟨re, im⟩`, ring operations, star involution, norm function, linear order (when d is nonsquare), integral domain and ordered ring instances, universal property via `lift`, units characterized by norm ±1 |
| GaussianInt.lean | Gaussian integers ℤ[i] = ℤ√(-1): embedding to ℂ, Euclidean division algorithm, Euclidean domain instance, characterization of representability as sums of two squares |
| QuadraticReciprocity.lean | Prime factorization in ℤ[i] via quadratic reciprocity: proves that a prime natural p is prime in ℤ[i] iff p ≡ 3 (mod 4) |
| ToReal.lean | Ring homomorphism from ℤ√d to ℝ (when d ≥ 0) using positive square root, injectivity when d is not a perfect square |

## Subdirectories

*(none)*

## Search Tags

quadratic-fields gaussian-integers zsqrtd norm euclidean-domain quadratic-reciprocity algebraic-integers linear-order integral-domain ring-homomorphism sums-of-squares complex-embedding real-embedding star-ring units primes-mod-four
