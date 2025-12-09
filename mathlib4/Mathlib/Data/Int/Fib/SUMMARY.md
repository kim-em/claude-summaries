---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Int/Fib
generated: 2025-12-09T10:37:15Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 2
subdirs_count: 0
---

# Fib

## Overview

The `Fib/` directory extends the Fibonacci sequence from natural numbers to integers. It defines `Int.fib` which satisfies the same recurrence relation as `Nat.fib` (F₀ = 0, F₁ = 1, Fₙ₊₂ = Fₙ₊₁ + Fₙ) but handles negative indices using parity-based formulas. The directory includes core properties of the integer Fibonacci sequence, addition formulas (including `fib_add` and doubling formulas), divisibility results (`fib_dvd`), GCD relationships, and classical identities like Cassini's and Catalan's.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `Int.fib` extending Fibonacci to integers; includes base cases (fib 0, fib 1, fib(-1), fib(-2)), handling of negative indices via parity, recurrence relations (fib_add_two, fib_add_one), addition formula `fib (m + n) = fib (m - 1) * fib n + fib m * fib (n + 1)`, doubling formulas, GCD theorem `gcd (fib m) (fib n) = Nat.fib (gcd m n)`, and divisibility properties |
| Lemmas.lean | Proves Cassini's identity `fib (n + 1) * fib (n - 1) - fib n ^ 2 = (-1) ^ \|n\|` and Catalan's identity `fib (x + a) ^ 2 - fib x * fib (x + 2 * a) = (-1) ^ \|x\| * fib a ^ 2` for integer Fibonacci numbers |

## Subdirectories

*(No subdirectories)*

## Search Tags

fibonacci integers fib negative-indices addition-formula doubling-formula cassini-identity catalan-identity divisibility gcd number-theory recurrence parity
