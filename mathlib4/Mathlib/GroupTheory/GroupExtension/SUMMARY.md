---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/GroupExtension
generated: 2026-01-24T22:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# GroupExtension

## Overview

The `GroupExtension/` directory formalizes the theory of group extensions as short exact sequences `1 → N → E → G → 1` (and their additive counterparts). Core structures include group extensions themselves, equivalences between extensions via commutative diagrams, sections (right inverses to the projection), splittings (section homomorphisms), and conjugacy relations on splittings. The directory establishes the connection between split extensions and semidirect products, showing that any split extension is equivalent to the extension associated with a semidirect product construction. This provides the foundation for classifying group extensions, with planned future work on connecting equivalence classes to group cohomology H² when N is abelian.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `GroupExtension N E G` structure (short exact sequence), `Equiv` (equivalences of extensions), `Section` (right inverses to projection), `Splitting` (section homomorphisms), `IsConj` (N-conjugacy relation), semidirect product to extension construction |
| Basic.lean | Basic lemmas and constructions: quotient isomorphisms, existence of sections, equivalence construction from homomorphisms, conjugation action, split extension equivalence to semidirect product, conjugacy classes of splittings |

## Subdirectories

*(none)*

## Search Tags

group-extension short-exact-sequence splitting section semidirect-product group-cohomology equivalence conjugacy quotient kernel-range exact-sequence extension-theory
