---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/PresentedMonoid
generated: 2025-12-04T08:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# PresentedMonoid

## Overview

The `PresentedMonoid/` directory provides the theory of monoids defined by generators and relations. Given a set of relations on the free monoid over a type α, it constructs the quotient monoid via congruence closure. This is a fundamental construction in abstract algebra for specifying monoids declaratively rather than constructively, analogous to how groups can be presented by generators and relators.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `PresentedMonoid rels` as quotient of free monoid by congruence closure of relations, with canonical map `of : α → PresentedMonoid rels`, universal property `lift` for extending maps that respect relations, induction principles, proof that generators generate the whole monoid, and extensionality lemmas; includes additive version `PresentedAddMonoid` |

## Subdirectories

*(no subdirectories)*

## Search Tags

presented-monoid generators relations monoid-presentation quotient congruence free-monoid universal-property additive-monoid group-presentation
