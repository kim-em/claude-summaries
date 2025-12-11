---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Set/Finite
generated: 2025-12-11T21:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 7
subdirs_count: 0
---

# Finite

## Overview

The `Finite/` directory contains the theory of finite sets in mathlib4. It provides three parallel layers of finiteness: `Fintype` instances (computable), `Finite` instances (classical), and `Set.Finite` constructors (proofs). The main file `Basic.lean` defines `Set.Finite.toFinset` to noncomputably convert a finite set proof to a `Finset`, along with `Fintype` instances for common set constructions (unions, intersections, images, inserts, etc.). Other files extend this to lattice operations on indexed unions/intersections, powerset finiteness, range finiteness, list operations, and monadic operations on sets.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core finite set theory: `Set.Finite.toFinset`, `Fintype` instances for union/intersection/image/insert/diff/singleton/empty, `Set.Finite` constructors for subset/union/image/preimage, induction principles for finite sets, cardinality lemmas, and properties of infinite sets |
| Lattice.lean | Finiteness of indexed unions and intersections: `Fintype`/`Finite`/`Set.Finite` results for `iUnion`, `sUnion`, `biUnion`, `iInter`; lattice-theoretic properties like `iSup_iInf_of_monotone`; bounded sets (`bddAbove`/`bddBelow`) for finite sets |
| Lemmas.lean | Additional lemmas assuming `Set.Finite`: embedding finite sets into `Fin n`, induction up to a finite set, existence of min/max images under linear orders |
| List.lean | Finiteness of sets of lists: `finite_length_eq`, `finite_length_lt`, `finite_length_le` for lists over a finite type |
| Monad.lean | Finiteness of Set monad operations: `Fintype`/`Finite`/`Set.Finite` for `bind`, `pure`, `seq`, and applicative operations on sets |
| Powerset.lean | Finiteness of powersets: `Set.Finite.finite_subsets` and `Set.Finite.powerset` proving the powerset of a finite set is finite |
| Range.lean | Finiteness of ranges: `fintypeRange` instance and `finite_range` constructor for ranges of functions from finite types |

## Subdirectories

(none)

## Search Tags

finite set fintype finset toFinset union intersection image preimage insert singleton iUnion biUnion sUnion iInter powerset range cardinality infinite bounded induction monad seq bind pure list
