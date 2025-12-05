---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Complex
generated: 2025-12-05T10:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 39
subdirs_count: 5
---

# Complex

## Overview

The `Complex/` directory provides a comprehensive formalization of complex analysis, establishing ℂ as a normed field and developing the classical theory of holomorphic and meromorphic functions. The directory contains fundamental theorems of complex analysis including Cauchy's integral formulas, Liouville's theorem, the maximum modulus principle, the open mapping theorem, Schwarz lemma, and the Phragmen-Lindelöf principle. It also covers removable singularities, conformal mappings, Taylor series convergence, and various complex analytic constructions.

Beyond general complex analysis, the directory includes specialized subdirectories for harmonic functions (satisfying Laplace's equation), complex polynomials (including the Fundamental Theorem of Algebra), the unit disc and upper half-plane as fundamental domains for geometric complex analysis, and Nevanlinna value distribution theory for measuring the complexity of meromorphic functions. Together, these components establish a foundation for further work in complex geometry, modular forms, and analytic number theory.

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

- [x] `Harmonic/` - Theory of harmonic functions satisfying Laplace's equation; proves harmonic functions are real-analytic (real parts of holomorphic functions) and satisfy the mean value property
- [x] `Polynomial/` - Complex polynomials including Fundamental Theorem of Algebra (ℂ is algebraically closed), Gauss-Lucas theorem on derivative roots, and irreducibility criteria for unit trinomials
- [x] `UnitDisc/` - Complex unit disc 𝔻 (Poincaré disc) as open unit ball in ℂ; algebraic structures, scalar actions by unit circle and closed ball, conjugation and projections
- [x] `UpperHalfPlane/` - Upper half-plane ℍ = {z : Im(z) > 0} with hyperbolic/Poincaré metric, GL(2,ℝ) and SL(2,ℤ) actions by Möbius transformations, smooth manifold structure, functions bounded at infinity (modular forms)
- [x] `ValueDistribution/` - Nevanlinna value distribution theory for meromorphic functions: characteristic function (height), counting function, proximity function, and First Main Theorem establishing invariance under function transformations

## Search Tags

complex-analysis holomorphic analytic cauchy-integral cauchy-theorem liouville-theorem maximum-modulus open-mapping schwarz-lemma phragmen-lindelof removable-singularity conformal-mapping taylor-series power-series entire-functions meromorphic residue-calculus circle-integral hadamard jensen-formula primitive-function abel-limit trigonometric exponential fourier-character harmonic-functions laplace-equation real-analytic mean-value-property fundamental-theorem-of-algebra algebraically-closed gauss-lucas-theorem polynomial-roots unit-disc poincare-disc upper-half-plane hyperbolic-geometry moebius-transformation modular-group GL2R SL2Z manifold-structure bounded-at-infinity modular-forms nevanlinna-theory value-distribution characteristic-function counting-function proximity-function first-main-theorem
