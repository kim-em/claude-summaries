---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Complex
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 39
subdirs_count: 5
---

# Complex

## Overview

The `Complex/` directory contains the formalization of complex analysis, including fundamental theorems about holomorphic functions, Cauchy's integral formulas, maximum modulus principles, and related results. It establishes the normed field structure on ℂ and develops the theory of complex differentiable functions with applications to analytic continuation, singularities, and conformal mappings. The directory includes classical results like Liouville's theorem, the open mapping theorem, Schwarz lemma, and the Phragmen-Lindelöf principle.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Normed space structure on ℂ; defines continuous linear maps (reCLM, imCLM, ofRealCLM, conjCLE, conjLIE) and establishes ℂ as a normed field and RCLike field |
| CauchyIntegral.lean | Cauchy-Goursat theorem and Cauchy integral formula for circles; proves analyticity of complex differentiable functions via power series expansions; includes formulas for higher derivatives |
| Liouville.lean | Liouville's theorem: bounded entire functions are constant; includes Cauchy's estimates for derivatives |
| AbsMax.lean | Maximum modulus principle in multiple versions; proves norm equality on connected sets when maximum is attained in interior |
| OpenMapping.lean | Open mapping theorem for holomorphic functions: non-constant analytic functions on connected sets are open maps |
| PhragmenLindelof.lean | Phragmen-Lindelöf principle (maximum modulus for unbounded domains) on strips, quadrants, and half-planes; includes extensionality lemmas |
| RemovableSingularity.lean | Riemann's removable singularity theorem: bounded functions on punctured neighborhoods extend to analytic functions |
| Schwarz.lean | Schwarz lemma and variants: bounds on derivatives and distances for functions mapping disks to disks |
| Exponential.lean | Complex exponential function and its analytical properties |
| Trigonometric.lean | Complex trigonometric functions (sin, cos, tan, etc.) and their properties |
| Circle.lean | The unit circle in ℂ as a submonoid, group, and topological group; exponential map from ℝ to circle; Fourier characters |
| TaylorSeries.lean | Convergence of Taylor series of holomorphic functions on balls and entire functions |
| Conformal.lean | Conformal mappings and their properties |
| Hadamard.lean | Hadamard's theorem and related results |
| JensenFormula.lean | Jensen's formula for holomorphic functions |
| LocallyUniformLimit.lean | Locally uniform limits of holomorphic functions |
| HasPrimitives.lean | Existence of primitives (antiderivatives) for holomorphic functions |
| AbelLimit.lean | Abel's limit theorem for power series |
| Angle.lean | Arguments and angles in complex analysis |
| Arg.lean | Argument function for complex numbers |
| Asymptotics.lean | Asymptotic behavior of complex functions |
| Cardinality.lean | Cardinality results for complex sets |
| Convex.lean | Convex sets in the complex plane |
| ExponentialBounds.lean | Bounds on the complex exponential function |
| HalfPlane.lean | Complex half-plane and its properties |
| IntegerCompl.lean | Complex plane minus integers |
| IsIntegral.lean | Integrality conditions for complex functions |
| Isometry.lean | Isometries on complex space |
| MeanValue.lean | Mean value properties for holomorphic functions |
| Norm.lean | Norm properties specific to complex analysis |
| OperatorNorm.lean | Operator norms for complex linear maps |
| Order.lean | Order-related properties in complex analysis |
| Periodic.lean | Periodic complex functions |
| Positivity.lean | Positivity extensions for complex analysis |
| ReImTopology.lean | Topology on ℂ via real and imaginary parts |
| RealDeriv.lean | Real derivatives of complex functions |
| Spectrum.lean | Spectral properties in complex analysis |
| SummableUniformlyOn.lean | Uniform summability on sets |
| Tietze.lean | Tietze extension theorem variants for complex functions |

## Subdirectories

- [x] `Harmonic/` - Harmonic functions (functions satisfying Laplace's equation) (complete)
- [x] `Polynomial/` - Complex polynomials and their analytical properties (complete)
- [x] `UnitDisc/` - Unit disc and related constructions (complete)
- [x] `UpperHalfPlane/` - Upper half-plane model and its properties (complete)
- [x] `ValueDistribution/` - Nevanlinna value distribution theory (characteristic, counting, proximity functions; First Main Theorem) (complete)

## Search Tags

complex-analysis holomorphic analytic cauchy-integral cauchy-theorem liouville-theorem maximum-modulus open-mapping schwarz-lemma phragmen-lindelof removable-singularity conformal-mapping taylor-series power-series entire-functions meromorphic residue-calculus circle-integral hadamard jensen-formula primitive-function abel-limit trigonometric exponential fourier-character harmonic-functions upper-half-plane unit-disc
