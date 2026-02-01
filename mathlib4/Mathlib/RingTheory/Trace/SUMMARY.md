---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Trace
generated: 2026-02-01T23:00:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Trace

## Overview

The `Trace/` directory contains the comprehensive theory of the trace map for ring extensions, particularly finite field extensions. The trace of an element is defined as the trace of the linear map given by multiplication, providing deep connections to minimal polynomials, Galois theory, and separability. The directory establishes fundamental properties (transitivity, relationship to field degree), advanced results connecting trace to roots of minimal polynomials and embeddings into algebraic closures, the trace form as a nondegenerate bilinear form over separable extensions, and specialized results for quotients and localizations in Dedekind domains.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of trace map `Algebra.trace R S : S →ₗ[R] R` as trace of multiplication operator, trace form as bilinear pairing, and trace matrix; proves tower law `Tr_{L/K}(Tr_{F/L} x) = Tr_{F/K} x`, trace of base ring elements is `[L:K] • x`, and basic computational lemmas |
| Basic.lean | Advanced trace theory: relates trace to sum of embeddings into algebraic closures `Tr(x) = ∑ σ x` for separable extensions; proves trace form is nondegenerate iff extension is separable; connection to minimal polynomial coefficients `Tr(gen) = -nextCoeff(minpoly)`; defines embeddings matrices and proves determinant of trace matrix is nonzero; constructs dual basis under trace form for separable extensions with explicit formula for power basis duals |
| Quotient.lean | Trace maps for quotients and localizations: proves trace commutes with quotient maps `Tr_{B/A}(x) ≡ Tr_{B/pB → A/p}(x̄) mod p` for Dedekind domains using integral trace; relates trace on quotients at maximal ideals to traces on localizations; key for arithmetic applications in number theory |

## Subdirectories

(none)

## Search Tags

trace-map ring-extension field-extension minimal-polynomial trace-form bilinear-form separable-extension Galois-theory algebraic-closure embeddings power-basis dual-basis nondegenerate-form quotient-ring localization Dedekind-domain integral-trace tower-law field-degree algebraic-element
