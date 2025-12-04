---
source_path: /Users/kim/Documents/Jobs/ANU/2015/1014/Notes
generated: 2025-12-04T06:00:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: preliminary
files_count: 7
subdirs_count: 25
---

# Notes

## Overview

Lecture notes for MATH1014 (Mathematics and Applications 2) semester 2 2015, containing 25 individual lecture directories with LaTeX source files for linear algebra topics. The folder includes a sophisticated build system using make and latexmk that automatically generates both presentation slides and 3-up handouts from each lecture's source. Key infrastructure files provide shared LaTeX formatting (beamer preamble, custom lecture document class, mathematical notation shortcuts) and build automation (makefile with targets for compilation and web posting).

## Key Files

| File | Purpose |
|------|---------|
| `makefile` | Complex build script that compiles all 25 lectures into slides and handouts, creates combined handout PDF, and posts to tqft.net website (2.7KB with automatic symbolic link creation and latexmk integration) |
| `beamer-preamble.tex` | Shared LaTeX preamble for beamer presentations (2.2KB with package imports for babel, graphics, AMS math, multicol) |
| `lecture.cls` | Custom LaTeX document class for lecture slides with automatic type detection (beamer/handout/slides) based on filename (2.4KB) |
| `local-defs.tex` | Mathematical notation macro definitions including vector commands (\vecx, \vecy), boldface shortcuts (\bi, \bj, \bk), and blackboard bold (\bR, \bZ, \bC) (3.3KB) |
| `course.tex` | Course metadata file defining MATH1014 title, instructor (Dr Scott Morrison), timing (Second Semester 2015), and institution (ANU MSI) (652 bytes) |
| `readme.txt` | Build instructions: 'make files' to recompile PDFs, 'make post' to upload to tqft.net (200 bytes) |
| `ignore` | Bash script for SVN version control that sets svn:ignore properties on LaTeX auxiliary files (aux, log, out, PDF, etc.) in all lecture directories (873 bytes) |

## Subdirectories

- [ ] `Lecture01/` - First lecture: Administrative overview and course introduction (pending)
- [ ] `Lecture02/` - Second lecture material (pending)
- [ ] `Lecture03/` - Third lecture material (pending)
- [ ] `Lecture04/` - Fourth lecture with additional examples file (potentially short per parent TODO note) (pending)
- [ ] `Lecture05/` - Fifth lecture material (pending)
- [ ] `Lecture06/` - Sixth lecture material (pending)
- [ ] `Lecture07/` - Seventh lecture material (pending)
- [ ] `Lecture08/` - Eighth lecture material (pending)
- [ ] `Lecture09/` - Ninth lecture material (pending)
- [ ] `Lecture10/` - Tenth lecture material (pending)
- [ ] `Lecture11/` - Eleventh lecture material (pending)
- [ ] `Lecture12/` - Twelfth lecture material (pending)
- [ ] `Lecture13/` - Thirteenth lecture material (pending)
- [ ] `Lecture14/` - Fourteenth lecture material (pending)
- [ ] `Lecture15/` - Fifteenth lecture material (pending)
- [ ] `Lecture16/` - Sixteenth lecture material (pending)
- [ ] `Lecture17/` - Seventeenth lecture material (pending)
- [ ] `Lecture18/` - Eighteenth lecture material (pending)
- [ ] `Lecture19/` - Nineteenth lecture material (pending)
- [ ] `Lecture20/` - Twentieth lecture material (pending)
- [ ] `Lecture21/` - Twenty-first lecture material (pending)
- [ ] `Lecture22/` - Twenty-second lecture material (pending)
- [ ] `Lecture23/` - Twenty-third lecture material (pending)
- [ ] `Lecture24/` - Twenty-fourth lecture with supplementary materials (SVD compression Mathematica notebook, Markov chain Python scripts, Harry Potter text, GIF/PNG images) (pending)
- [ ] `Lecture25/` - Final lecture material (pending)

## Search Tags

math1014 linear-algebra lecture-notes anu 2015 semester-2 beamer latex slides handouts pdf-generation build-system makefile latexmk scott-morrison mathematics first-year teaching
