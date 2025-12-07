---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Galois
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 12
subdirs_count: 0
---

# Galois

## Overview

The `Galois/` directory contains the formalization of Galois categories and their fundamental theorem following SGA1. Galois categories are categorical abstractions that capture the essential features of the category of finite étale covers and finite Galois extensions, providing a framework for studying fundamental groups in algebraic topology and algebraic geometry. The implementation defines PreGalois categories (categories satisfying axioms G1-G3), fiber functors (axioms G4-G6), and proves the fundamental theorem: any fiber functor induces an equivalence with the category of finite discrete actions of its automorphism group.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of PreGaloisCategory and FiberFunctor following Lenstra's axiomatization (G1-G6) with connected objects |
| GaloisObjects.lean | Galois objects defined as connected objects whose quotient by automorphisms is terminal, with transitive action characterization |
| Action.lean | Induced functor from Galois categories to finite Aut F-sets with preservation and reflection properties |
| Full.lean | Fullness of the induced functor to Aut F-sets via lifting subobjects and connectedness preservation |
| EssSurj.lean | Essential surjectivity showing the essential image consists of finite discrete Aut F-sets with continuous actions |
| Equivalence.lean | Main theorem: fiber functors induce equivalence with category of finite discrete Aut F-sets |
| Prorepresentability.lean | Pro-representability of fiber functors via pointed Galois objects with Aut F as limit of automorphism groups |
| Decomposition.lean | Decomposition of objects into finitely many connected components with Galois representatives for fibers |
| Topology.lean | Natural topology on Aut F as subspace topology from product of discrete automorphism groups of fibers |
| IsFundamentalgroup.lean | Universal property identifying when a topological group is canonically isomorphic to Aut F via transitive actions |
| Examples.lean | Finite G-sets as PreGalois category with forgetful functor to FintypeCat as fiber functor |

## Subdirectories

(none)

## Search Tags

galois-categories fiber-functors fundamental-group automorphism-groups galois-objects connected-objects pretransitive-actions fundamental-theorem pro-representability pointed-objects decomposition etale-covers galois-theory algebraic-topology compact-topological-groups
