---
source_path: /Users/kim/Documents/CV
generated: 2025-12-01T20:15:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 51
subdirs_count: 5
---

# CV

## Overview

Comprehensive academic curriculum vitae materials for Kim Morrison spanning a career from UC Berkeley PhD (under Vaughan Jones) through current role at Lean FRO. The directory contains LaTeX source files and compiled PDFs for multiple CV variants including full resume, one-page condensed version, publications list, research statement, and teaching statement. Build infrastructure includes Ant scripts and specialized diagram processing pipelines. Supporting materials document academic achievements: university transcripts with UNSW Medal, Herbert Alexander Prize certificate, referee reports from major publications in Acta Mathematica and other top journals. The media subdirectory captures Morrison's public engagement through the pivotal 2013 Polymath 8 prime gaps project and 2018 blackboard advocacy at ANU. Historical versions preserve earlier career documents and prize nominations. The sections subdirectory provides modular LaTeX components including a comprehensive 40+ paper publications list (2006-2023) and personal climbing achievements. Business card designs and mathematical diagram assets (Temperley-Lieb algebra, knot diagrams) complete the portfolio infrastructure.

## Key Files

| File | Purpose |
|------|---------|
| `resume.tex` | Main LaTeX source for comprehensive CV covering employment at Lean FRO (2023-present), ANU professorship (2012-2020), Miller Fellowship at Berkeley, Station Q postdoc, prizes (AMS Medal, Heyde Medal), PhD from Berkeley under Vaughan Jones, grants, service, and media appearances |
| `resume.pdf` | Compiled resume (90KB, last built April 2024) |
| `resume-1-page.tex` | Condensed one-page version of resume |
| `resume-1-page.pdf` | Compiled one-page resume (251KB) |
| `publications.tex` | LaTeX wrapper including publications list from `sections/publications.tex` |
| `publications.pdf` | Compiled publications list (71KB) with reference to http://tqft.net/web/publications |
| `research-statement.tex` | Detailed research statement (24KB LaTeX source) covering TQFT, Khovanov homology, 4-dimensional geometry, subfactors, fusion categories, and topological quantum computing |
| `research-statement.pdf` | Compiled research statement (37KB) |
| `teaching-statement.tex` | Teaching philosophy statement from early career (postdoc period), discussing teaching experience, collaboration with graduate students, and interest in incorporating computer algebra into mathematics teaching |
| `teaching-statement.pdf` | Compiled teaching statement (19KB) |
| `preamble.tex` | Shared LaTeX preamble with packages, theorem environments, hyperref setup, color definitions, custom commands for arXiv/DOI/MathSciNet links, and page layout settings |
| `header.tex` | Contact header for CV documents showing current position at Lean FRO, phone number, and email |
| `referee-reports.txt` | Selected excerpts from peer review reports for major publications in Acta Mathematica, Communications in Mathematical Physics, Geometry & Topology, and Transactions of the AMS, highlighting significance of work on blob complex, extended Haagerup planar algebra, subfactor classification, and fusion categories |
| `build.xml` | Ant build script for LaTeX compilation |
| `ant-eps-diagrams.bat` | Windows batch file for diagram processing |
| `Herb_Alexander_Prize.pdf` | Certificate for 2007 Herbert Alexander Prize for Outstanding Dissertation in Pure Mathematics from UC Berkeley |
| `UNSW Diploma & Transcript.pdf` | University of New South Wales diploma and transcript (237KB) showing BSc Honours with University Medal (1998-2001) |
| `publications-Heyde-medal-nomination-2014.tex` | Publications list formatted for Heyde Medal nomination (2014) |
| `publications-Heyde-medal-nomination-2014.pdf` | Compiled Heyde Medal nomination publications (324KB) |
| `publications-DAAD-2014.tex` | Publications list for DAAD application (2014) |
| `research-statement-subfactors.tex` | Specialized research statement focused on subfactors (5KB) |
| `resume-Heyde-medal-nomination-2014.tex` | Resume version for Heyde Medal nomination |
| `resume-Heyde-medal-nomination-2014.pdf` | Compiled Heyde Medal nomination resume (271KB) |
| `*.aux`, `*.bbl`, `*.blg`, `*.log`, `*.out`, `*.dvi`, `*.ps` | LaTeX build artifacts from compilation process (April 2024 build) |

## Subdirectories

- [x] `business-card/` - Business card design files including Adobe Illustrator sources, ANU logo, QR code, photos (chalkboard, slate), and associahedron diagram
- [x] `diagrams/` - Complete mathematical diagram asset pipeline with Temperley-Lieb algebra and knot diagram primitives in EPS/PDF formats, plus build automation for LaTeX dependency detection and incremental conversion, and specialized latex2pdf workflow for Illustrator-editable defontified vectors
- [x] `historical/` - Historical versions of CV materials including 2008 research statement, teaching statement, and UNSW transcripts and prize certificates
- [x] `media/` - Media coverage focusing on Polymath 8 prime gaps collaboration (2013, including Morrison's pivotal blog post that sparked the project) and ANU blackboard advocacy (2018, featuring imported Hagoromo Fulltouch chalk), with coverage from Simons Foundation, New York Times, New Scientist, The Hindu, and Canberra Times
- [x] `sections/` - Modular LaTeX sections for inclusion in main CV documents: comprehensive publications list (40+ papers spanning 2006-2023 in subfactors, fusion categories, Khovanov homology) and climbing achievements section documenting alpine and big wall ascents including El Capitan one-day climbs

## Search Tags

curriculum-vitae resume academic-cv latex publications research-statement teaching-statement kim-morrison lean-fro anu-professor subfactors fusion-categories topological-quantum-computing khovanov-homology vaughan-jones miller-fellowship station-q heyde-medal ams-medal mathoverflow mathematical-physics berkeley unsw theorem-proving academic-portfolio career-documents
