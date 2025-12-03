---
source_path: /Users/kim/Documents/CV/diagrams/scripts
generated: 2025-12-01T18:50:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 9
subdirs_count: 0
---

# scripts

## Overview

Build automation scripts for converting PDF diagrams to EPS format for LaTeX inclusion. Provides dependency detection by parsing LaTeX sources for diagram references (`\mathfig`, `\placefig`, `\rotatemathfig` commands), incremental conversion using Ghostscript at 2400 DPI with timestamp-based staleness checks, and cross-platform support via both bash and batch wrappers. The workflow maintains `diagrams.list` (auto-discovered) and `extra_diagrams.list` (manual additions) to track which diagrams need conversion.

## Key Files

| File | Purpose |
|------|---------|
| `README.txt` | Documentation explaining the build workflow: find_all_diagrams discovers dependencies, stripall converts PDF to EPS for non-pdflatex workflows |
| `find_all_diagrams.sh` | Scans all .tex files in parent directories (root and sections/) and runs find_diagrams.sh on each to populate diagrams.list |
| `find_diagrams.sh` | Extracts diagram filenames from LaTeX commands (\mathfig, \placefig, \rotatemathfig) using grep and sed, appends to diagrams.list |
| `stripall.sh` | Main conversion script: processes diagrams from both lists, checks modification times, calls strippdf.sh only for stale diagrams |
| `strippdf.sh` | Ghostscript wrapper: converts single PDF to EPS at 2400 DPI, strips CreationDate metadata for reproducible builds |
| `find_all_diagrams.bat` | Windows batch wrapper that invokes find_all_diagrams.sh via bash |
| `stripall.bat` | Windows batch wrapper that invokes stripall.sh via bash |
| `diagrams.list` | Auto-generated list of diagram basenames found in LaTeX sources (8 entries: crossing, vertical, horizontal, spaghetti, torus, cut1, cut2) |
| `extra_diagrams.list` | Manual override file for diagrams not automatically discovered (currently empty) |

## Subdirectories

No subdirectories.

## Search Tags

build-automation pdf-to-eps ghostscript latex-workflow diagram-conversion dependency-detection incremental-build makefile-replacement cross-platform bash-scripts windows-batch reproducible-builds metadata-stripping timestamp-based-staleness 2400-dpi eps-generation latex-figures mathfig placefig rotatemathfig sed-parsing grep-extraction
