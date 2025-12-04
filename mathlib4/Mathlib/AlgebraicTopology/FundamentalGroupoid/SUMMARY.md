---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/FundamentalGroupoid
generated: 2025-12-04T08:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# FundamentalGroupoid

## Overview

This folder formalizes the fundamental groupoid of a topological space and the fundamental group. The fundamental groupoid has points as objects and homotopy classes of paths as morphisms, forming a groupoid structure. Key results include the fundamental group as the automorphism group of a basepoint, functoriality of the fundamental groupoid construction, product preservation, and characterizations of simply connected spaces.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of the fundamental groupoid structure on a topological space, with objects as points and morphisms as path homotopy classes; proves groupoid laws (identity, composition, associativity, inverses) and defines the fundamental groupoid functor π : TopCat → Grpd |
| FundamentalGroup.lean | Defines the fundamental group π₁(X, x) as the automorphism group (vertex group) of a basepoint in the fundamental groupoid; provides isomorphisms between fundamental groups at different basepoints via path conjugation, including the canonical isomorphism for path-connected spaces |
| InducedMaps.lean | Shows homotopic continuous maps induce naturally isomorphic functors between fundamental groupoids; proves homotopy equivalent spaces have equivalent fundamental groupoids; establishes the key diagram relating path images under homotopic maps via the diagonal path construction |
| PUnit.lean | Proves the fundamental groupoid of the one-point space PUnit is equivalent to the discrete groupoid on PUnit; uses subsingletonness of paths in PUnit to establish the equivalence |
| Product.lean | Proves the fundamental groupoid functor preserves products; establishes isomorphisms π(Π i, Xᵢ) ≅ Π i, π(Xᵢ) and π(X × Y) ≅ π(X) × π(Y), with inverses given by induced projection maps; formally verifies the fundamental groupoid functor preserves limits |
| SimplyConnected.lean | Defines simply connected spaces as those whose fundamental groupoid is equivalent to the discrete groupoid on Unit; proves equivalence with unique path homotopy classes, path-connectedness with subsingleton path homotopy, and null-homotopic loops; shows contractible spaces are simply connected |

## Subdirectories

(No subdirectories)

## Search Tags

fundamental-groupoid fundamental-group path-homotopy groupoid-category topological-space homotopy-theory path-connected simply-connected contractible-space automorphism-group vertex-group functor-preservation product-preservation homotopy-equivalence natural-isomorphism loops basepoint conjugation discrete-groupoid
