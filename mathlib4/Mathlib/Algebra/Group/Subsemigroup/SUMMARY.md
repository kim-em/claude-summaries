---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Subsemigroup
generated: 2025-12-01T21:40:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Subsemigroup

## Overview

The `Subsemigroup/` directory provides the complete theory of subsemigroups, the most basic substructure in algebra. A subsemigroup is simply a subset closed under multiplication—requiring neither associativity, identity, nor inverses from the ambient structure (only `Mul M`). This minimal foundation makes subsemigroups the first layer in the algebraic substructure hierarchy. The directory develops four key aspects: core definitions with bundled structures and membership typeclasses (`Defs.lean`), a complete lattice structure with closure operators and Galois insertions (`Basic.lean`), membership characterizations for directed suprema with induction principles (`Membership.lean`), and operations including maps, products, and conversions between multiplicative and additive forms (`Operations.lean`). The design emphasizes minimal dependencies, avoiding even natural numbers, to serve as a foundation for higher algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Foundational definitions: bundled `Subsemigroup M` and `AddSubsemigroup M` structures with carriers closed under operations; `MulMemClass`/`AddMemClass` typeclasses for generic subsemigroup predicates; basic lattice instances (⊤, ⊥, ⊓); `SetLike` interface for subset coercion; `MulHom.eqLocus` equalizer construction; extensionality and copy lemmas; explicitly avoids dependencies on natural numbers and complete lattices |
| Basic.lean | Complete lattice structure: `CompleteLattice` instance for subsemigroups built from infimum; `Subsemigroup.closure` as minimal subsemigroup containing a set with Galois insertion properties; multiple induction principles (`closure_induction`, `closure_induction₂`, `dense_induction`) for reasoning about closure; lattice operations (sInf, iInf, suprema via closure, unions); `MulHom.ofDense` for extending homomorphisms from dense subsets; monotonicity and closure characterization lemmas |
| Membership.lean | Membership characterization for suprema: directed suprema of subsemigroups equal their unions (`mem_iSup_of_directed`, `coe_iSup_of_directed`, `mem_sSup_of_directed_on`); induction principles for elements of suprema (`iSup_induction`, `iSup_induction'` with dependent types); basic membership lemmas for binary suprema (`mem_sup_left`, `mem_sup_right`, `mul_mem_sup`); stub file intended to mirror `Submonoid.Membership` structure |
| Operations.lean | Operations and morphisms: `Subsemigroup.comap` (preimage) and `map` (image) with Galois connection/insertion properties; `Subsemigroup.prod` for Cartesian products with equivalence to product type; conversions between multiplicative and additive via `toAddSubsemigroup`/`toSubsemigroup` order isomorphisms; `MulHom.srange` (range as subsemigroup), `restrict`, `codRestrict`; subsemigroup inclusion maps and equivalences (`subsemigroupCongr`, `prodEquiv`); inherited semigroup/commutative structures on subsemigroup subtypes |

## Subdirectories

(none)

## Search Tags

subsemigroup additive-subsemigroup closure lattice complete-lattice galois-insertion map comap product range membership directed-suprema induction-principle mul-mem-class additive-multiplicative-conversion homomorphism magma substructure minimal-dependencies equalizer dense-subset semigroup-structure
