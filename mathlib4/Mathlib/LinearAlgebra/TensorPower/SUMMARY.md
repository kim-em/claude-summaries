---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/TensorPower
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# TensorPower

## Overview

The `TensorPower/` directory defines tensor powers of modules as special cases of pi tensor products, where the n-th tensor power `⨂[R]^n M` is the n-ary tensor product indexed by `Fin n`. The directory establishes graded algebraic structures (graded monoid, graded semiring, graded algebra) on direct sums of tensor powers, proving that tensor powers form a graded semiring with multiplicative structure given by concatenation. It also covers the pairing between tensor powers of duals and duals of tensor powers, and introduces symmetric tensor powers as quotients by permutation equivalence.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core tensor power theory: abbreviation `TensorPower R n M := ⨂[R] i : Fin n, M` with notation `⨂[R]^n M`, graded multiplicative structure (`gOne`, `gMul`, `gmonoid` instances), multiplication via `mulEquiv` reindexing `⨂[R]^n M ⊗[R] ⨂[R]^m M ≃ₗ[R] ⨂[R]^(n+m) M`, casting between equal tensor powers, graded semiring structure (`DirectSum.GSemiring`), and graded algebra structure (`DirectSum.GAlgebra`) with algebra map from R to ⨂[R]^0 M |
| Pairing.lean | Dual pairing for tensor powers: multilinear map `multilinearMapToDual` from n copies of dual Module.Dual R M to dual of tensor power Module.Dual R (⨂[R]^n M), canonical linear map `pairingDual : ⨂[R]^n (Module.Dual R M) →ₗ[R] (Module.Dual R (⨂[R]^n M))`, evaluation formula `pairingDual (tprod f) (tprod v) = ∏ i, f i (v i)` computing pairing as product of individual evaluations |
| Symmetric.lean | Symmetric tensor powers: equivalence relation `SymmetricPower.Rel` identifying tensors related by permutations, quotient construction `SymmetricPower R ι M` (notation `Sym[R] ι M`) as additive congruence quotient, module structure via permutation-respecting scalar multiplication, canonical quotient map `mk : ⨂[R] ι M →ₗ[R] Sym[R] ι M`, multilinear constructor `tprod : MultilinearMap R (fun _ : ι ↦ M) Sym[R] ι M` (notation `⨂ₛ[R] i, f i`), permutation invariance `tprod_equiv`, and spanning property `span_tprod_eq_top` |

## Subdirectories

(none)

## Search Tags

tensor-power tensor-product graded-algebra graded-monoid graded-semiring pi-tensor-product direct-sum multilinear symmetric-tensor dual-pairing permutation-invariant algebraMap concatenation reindex fin commutative-semiring module linear-equiv quotient congruence
