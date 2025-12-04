---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/LocalExtr
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# LocalExtr

## Overview

The `LocalExtr/` directory formalizes the theory of local extrema (maxima and minima) for differentiable functions. It proves Fermat's Theorem (derivatives vanish at local extrema) in multiple variants: for Fréchet derivatives, ordinary derivatives, and line derivatives. The directory also proves Rolle's Theorem (existence of critical points between equal function values) and applies it to count polynomial roots. A key technical tool is the positive tangent cone, which captures directions along which functions can be approached within constraint sets—essential for constrained optimization and Lagrange multipliers.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of local extrema: defines positive tangent cone `posTangentConeAt` for constraint directions; proves Fermat's Theorem (derivative equals zero at local extrema) for both Fréchet derivatives and ordinary derivatives; includes constrained versions (derivative vanishes in tangent cone directions) |
| LineDeriv.lean | Extends Fermat's Theorem to line derivatives (directional derivatives): proves line derivatives vanish at local extrema, both globally and on constraint sets |
| Rolle.lean | Proves Rolle's Theorem in four variants: if continuous f has equal values at interval endpoints and is differentiable in between, then derivative vanishes somewhere in the interior; includes both `HasDerivAt` and `deriv` versions, and limit-based versions for open intervals |
| Polynomial.lean | Applies Rolle's Theorem to polynomial root counting: proves the number of real roots of a polynomial is at most the number of roots of its derivative plus one (both with and without multiplicity); uses interleaving argument via Rolle's Theorem |

## Subdirectories

*(None)*

## Search Tags

local-extrema fermat-theorem critical-points derivative-vanishes rolle-theorem polynomial-roots tangent-cone constrained-optimization line-derivatives directional-derivatives root-counting maxima minima stationary-points
