---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Operator
generated: 2025-12-05T11:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 17
subdirs_count: 0
---

# Operator

## Overview

The `Operator/` directory contains the comprehensive theory of bounded linear operators (continuous linear maps) between normed spaces. It provides the fundamental operator norm structure, proves that continuous linear maps form a normed space, and establishes major theorems of functional analysis including the Banach open mapping theorem, the Banach-Steinhaus uniform boundedness principle, and theory of compact operators. The directory covers linear and semilinear maps, linear isometries and isometric equivalences, bounded bilinear maps, completeness properties, and extension theorems for continuous linear maps from dense subspaces.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines operator (semi-)norm on continuous (semi)linear maps between (semi)normed spaces; proves space of operators is itself seminormed; shows surjectivity is equivalent to containing a ball; handles continuity and boundedness equivalence |
| ContinuousLinearMap.lean | Core constructions of continuous linear maps; `LinearMap.mkContinuous` builds continuous map from linear map + bound; proves boundedness implies continuity; fundamental infrastructure for continuous linear maps |
| LinearIsometry.lean | Defines semilinear isometric embeddings (`E →ₛₗᵢ[σ₁₂] E₂`) and isometric equivalences (`E ≃ₛₗᵢ[σ₁₂] E₂`); linear isometries preserve norm exactly (`‖f x‖ = ‖x‖`); includes star-linear versions; basic properties and constructors |
| Banach.lean | Banach open mapping theorem: bijective bounded linear map between Banach spaces has bounded inverse; defines `NonlinearRightInverse` structure for nonlinear but bounded right inverses; fundamental result for surjective continuous linear maps |
| BanachSteinhaus.lean | Banach-Steinhaus uniform boundedness principle: pointwise bounded family of continuous linear maps from Banach space is uniformly bounded; includes `continuousLinearMapOfTendsto` for limits of operator sequences |
| BoundedLinearMaps.lean | Defines `IsBoundedLinearMap` (unbundled continuous linear map) and `IsBoundedBilinearMap` (continuous bilinear map with `‖f(x,y)‖ ≤ C‖x‖‖y‖`); includes derivatives of bilinear maps; shows continuous linear equivalences form open set |
| Bilinear.lean | Operator norm theory for bilinear maps `E × F → G` interpreted as `E → F → G`; norm estimates and properties for composition of continuous linear maps with bilinear structure |
| Compact.lean | Compact operators between topological vector spaces; `IsCompactOperator` predicate for operators with precompact image of neighborhoods; proves compact operators are continuous and form closed set; fundamental for spectral theory |
| Completeness.lean | Operator norm on complete normed spaces; Banach-Alaoglu theorem (`isCompact_image_coe_closedBall`); completeness properties of operator spaces; constructions requiring complete domain or codomain |
| Extend.lean | Extension theorems for continuous linear maps from dense subspaces to Banach spaces; `ContinuousLinearMap.extend` and `LinearMap.extendOfNorm` extend bounded maps from dense embeddings; `LinearEquiv.extendOfIsometry` extends isometries |
| NormedSpace.lean | Operator norm for maps on normed spaces (not just seminormed); statements requiring actual norm (not just seminorm); `LinearMap.bound_of_shell` for establishing boundedness from local bounds |
| NNNorm.lean | Non-negative operator norm (`‖f‖₊ : ℝ≥0`); properties of operator norm as element of `ℝ≥0`; compatibility between `‖f‖` and `‖f‖₊` |
| Mul.lean | Multiplicative properties of operator norm; composition of continuous linear maps and norm estimates; `‖f ∘ g‖ ≤ ‖f‖ * ‖g‖` |
| Prod.lean | Continuous linear maps on product spaces; constructions for `E × F` as domain or codomain; projections and diagonal maps |
| CompleteCodomain.lean | Properties of continuous linear maps with complete codomain; constructions and theorems requiring codomain completeness |
| Asymptotics.lean | Asymptotic behavior of continuous linear maps; big-O and little-o properties; landau notation for operators |
| Conformal.lean | Conformal maps between normed spaces; maps that preserve angles; relationship with isometries and scalar multiplication |

## Subdirectories

(None - this is a leaf directory)

## Search Tags

bounded-linear-operators continuous-linear-maps operator-norm functional-analysis banach-spaces linear-isometries banach-open-mapping-theorem banach-steinhaus uniform-boundedness compact-operators bilinear-maps semilinear-maps completeness extension-theorems dense-subspaces nonlinear-inverse isometric-equivalence asymptotic-analysis conformal-maps operator-composition seminormed-spaces normed-spaces bounded-maps
