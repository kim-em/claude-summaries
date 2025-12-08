---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Quiver
generated: 2025-12-08T23:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 13
subdirs_count: 1
---

# Quiver

## Overview

The `Quiver/` directory contains a comprehensive formalization of quivers (directed multigraphs) in Lean. A quiver on type `V` assigns to every pair of vertices `a b : V` a type `a ⟶ b` of arrows between them. This is a very permissive notion of directed graph that allows multiple edges and serves as the foundation for category theory. The directory includes theory for paths, connectivity, symmetrization, subquivers, morphisms (prefunctors), arborescences (directed rooted trees), and covering maps.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core quiver definition: `Quiver` typeclass mapping vertex pairs to arrow types, with notation `a ⟶ b`; includes opposite quivers, empty quivers, thin quivers (no parallel arrows), and `homOfEq` for transporting arrows across equalities |
| Path.lean | Inductive path type `Path a b` representing sequences of composable arrows; includes path composition, length, decomposition lemmas, decidable equality for bounded paths, and conversion to/from lists; defines `BoundedPaths` for paths with uniform length bounds |
| Prefunctor.lean | Morphisms between quivers: `Prefunctor V W` with object map `obj : V → W` and arrow map `map`; includes identity, composition, extensionality, and notation `V ⥤q W` (extends to categorical functors later) |
| Arborescence.lean | Directed rooted trees: `Arborescence V` typeclass asserting unique path from root to every vertex; includes `arborescenceMk` constructor using height functions, `RootedConnected` typeclass, and `geodesicSubtree` construction proving every rooted connected quiver has a spanning arborescence |
| ConnectedComponent.lean | Weak and strong connectivity: `WeaklyConnectedComponent` (zigzag quotient via symmetrified paths), `StronglyConnectedComponent` (bidirectional reachability quotient), `IsStronglyConnected` (paths between all pairs), and `IsSStronglyConnected` (positive-length paths between all pairs) |
| Symmetric.lean | Symmetrization and reversal: `Symmetrify V` adds formal inverses to arrows (`(a ⟶ b) ⊕ (b ⟶ a)`), `HasReverse` and `HasInvolutiveReverse` typeclasses for arrow reversal, `Path.reverse` for reversing paths, and `Prefunctor.MapReverse` for functors preserving reversal |
| Covering.lean | Covering maps: defines `Quiver.Star u` (arrows from u) and `Quiver.Costar u` (arrows to u); `Prefunctor.IsCovering φ` means φ induces bijections on all stars/costars; proves covering functors give bijections on path spaces (unique path lifting) |
| Subquiver.lean | Subquivers as predicates on arrows: `WideSubquiver` and `TotalSubquiver` with induced quiver structures; includes lattice operations, subquiver membership, and coercion to quivers |
| Cast.lean | Type-changing operations for quivers: casting quiver structures and arrows along type equalities; includes `PushQuiver` for changing vertex types via functions |
| Push.lean | Push-forward construction: given function `σ : V → V'`, construct `Push σ` quiver with vertices `V'` and arrows from pushed quiver structure; includes universal property via `Push.of` prefunctor |
| ReflQuiver.lean | Reflexive quivers with identity arrows: `ReflQuiver` typeclass extending `Quiver` with `id : a ⟶ a` for all vertices; includes reflexive closure construction and prefunctors preserving identities |
| SingleObj.lean | Single-object quivers from monoids: `SingleObj α` wraps type `α` as single vertex with arrows from monoid structure; establishes quiver-monoid correspondence |
| Subquiver.lean | Subquiver predicates and lattice structure: wide subquivers (all vertices, predicate on arrows) and total subquivers (predicate on both); includes closure operators and induced quiver instances |

## Subdirectories

- [x] `Path/` - Additional path theory: decomposition, vertices, and weight (complete)

## Search Tags

quiver directed-multigraph category-theory arrows vertices paths composition prefunctor arborescence connectivity strongly-connected weakly-connected symmetrify reversal covering star costar subquiver reflexive push-forward
