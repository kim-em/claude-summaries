---
source_path: /Users/kim/.claude/statsig
generated: 2025-12-02T10:48:00Z
git_sha: ebe831cc1718246ffc866d2d1603aea2fc46574a
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# statsig

## Overview

Statsig client cache for feature flags and A/B testing configuration used by Claude Code. Contains cached feature gate evaluations (50+ gates), dynamic configs (30+ experiments), session identifiers, and last-modified timestamps. This enables offline feature flag evaluation and reduces network requests to Statsig servers.

## Key Files

| File | Purpose |
|------|---------|
| statsig.cached.evaluations.d93183bdae | Cached feature gates and dynamic configs from Statsig API (~23KB JSON with 50+ feature flags, 30+ experiments) |
| statsig.session_id.2656274335 | Current session identifier with start time and last update timestamp |
| statsig.stable_id.2656274335 | Stable user identifier UUID persisted across sessions |
| statsig.last_modified_time.evaluations | Timestamp tracking when cached evaluations were last fetched (epoch milliseconds) |

## Subdirectories

*(No subdirectories)*

## Search Tags

statsig feature-flags ab-testing experiments cache telemetry client-sdk configuration dynamic-config
