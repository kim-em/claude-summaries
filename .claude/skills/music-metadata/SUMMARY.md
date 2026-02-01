---
source_path: /Users/kim/.claude/skills/music-metadata
generated: 2026-02-01T14:00:00Z
git_sha: 5ab0a683024feca845347c2f155eaf4d2e8ceb52
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# music-metadata

## Overview

A Claude Code skill for identifying unknown music albums using audio fingerprinting and applying proper metadata tags. Provides a comprehensive workflow using beets with chromaprint/AcoustID integration for automatic identification, with fallback to manual tagging via mid3v2 when albums aren't in the MusicBrainz database. Includes guidance for when identification fails (asking the user first, then MusicBrainz lookup, then manual tagging).

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Complete skill definition covering prerequisites (chromaprint, beets+pyacoustid, mutagen/mid3v2), beets configuration, identification workflow (preview with verbose mode), tag application, verification, and extensive fallback procedures for unidentified albums including manual mid3v2 tagging with cover art embedding |

## Subdirectories

None.

## Search Tags

music-metadata audio fingerprinting chromaprint acoustid beets musicbrainz tagging mp3 id3 mid3v2 mutagen album identification cd-ripping unknown-album cover-art genre track-numbering pyacoustid fpcalc
