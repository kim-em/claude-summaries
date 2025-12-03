---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Field/Subfield
generated: 2025-12-01T19:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Subfield

## Overview

The `Subfield/` directory defines the bundled subfield type `Subfield K` for division rings `K`, representing sub-division rings (skew fields) that need not be commutative. It provides a complete lattice structure on subfields with operations like closure, map/comap along ring homomorphisms, and proves that closure forms a Galois insertion with set coercion. The directory implements subfields as subrings closed under multiplicative inverses, with comprehensive theory for working with subfield membership, lattice operations, and ring homomorphism interactions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `SubfieldClass` type class, `Subfield` structure (as subring + inverse closure), rational casting, scalar multiplication instances, and automatic `DivisionRing`/`Field` instances for subfields |
| Basic.lean | Comprehensive subfield theory: complete lattice structure, `closure` construction (Galois insertion), `map`/`comap` operations, `fieldRange` for ring homomorphisms, `eqLocusField` (equalizer), inclusion homomorphisms, and specialized lemmas for commutative fields |

## Subdirectories

(none)

## Search Tags

subfield subfields division-ring skew-field closure galois-insertion map comap fieldrange complete-lattice ring-homomorphism subring inverse-closure subfieldclass eq-locus inclusion bundled-subfield
