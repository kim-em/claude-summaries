---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic/Godel
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Godel

## Overview

The `Godel/` directory contains a proof of Gödel's Beta Function Lemma, a key technical result used in the proof of Gödel's First Incompleteness Theorem. The Beta Function provides a way to encode and decode finite sequences of natural numbers in a manner that is arithmetically definable, enabling quantification over sequences in formal theories of arithmetic. This is separate from the Beta Function in analysis and provides similar functionality to `Encodable.encodeList`/`decodeList` but with easier-to-prove arithmetic definability.

## Key Files

| File | Purpose |
|------|---------|
| GodelBetaFunction.lean | Defines `Nat.beta` (Gödel's Beta Function for decoding sequences) and `Nat.unbeta` (encoding sequences); proves the main result `beta_unbeta_coe` (Gödel's Beta Function Lemma) showing that decoding after encoding recovers the original sequence; uses Chinese Remainder Theorem with carefully constructed pairwise coprime moduli based on factorials; implementation originated from https://github.com/iehality/lean4-logic repository by Shogo Saito, adapted for mathlib by Hunter Monroe |

## Subdirectories

None

## Search Tags

godel beta-function incompleteness-theorem arithmetic-definability encoding chinese-remainder-theorem logic metamathematics peano-arithmetic sequences
