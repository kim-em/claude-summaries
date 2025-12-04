---
source_path: /Users/kim/Documents/Jobs/ANU/2015/1014/Notes/Lecture12/diagrams
generated: 2025-12-04T06:30:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: complete
files_count: 10
subdirs_count: 0
---

# diagrams

## Overview

Supporting materials for Lecture 12 Markov chains topic, containing Maple computational worksheets (.mw files) that demonstrate matrix power calculations for transition matrices, and presentation slides (PDF) explaining Markov chains theory from Lay §4.9. The folder includes worked examples of the "Weather in the Land of Oz" problem showing probability state vector evolution, both in exact fractional form and decimal approximations. One OmniGraffle diagram file and an additional PDF (prova.pdf, likely from Semester 2, 2011) provide visual aids for the lecture material.

## Key Files

| File | Purpose |
|------|---------|
| `map1301.mw` | Maple worksheet (4.8KB) computing T^7*x0 for Markov chain transition matrix T with fractional entries, demonstrating exact rational arithmetic for probability calculations (output: state vector with entries 3277/16384, 3277/8192, 6553/16384) |
| `map1302.mw` | Maple worksheet (4.9KB) computing same T^7*x0 calculation but using decimal matrix entries (0.25, 0.5, etc.), producing floating-point approximations (output: 0.2000122070, 0.4000244140, 0.3999633789) |
| `map1303.mw` | Maple worksheet (7.9KB) with additional Markov chain computations (larger file suggests more extensive calculations or multiple examples) |
| `la1301.pdf` | Maple output showing transition matrix T setup and T^7*x0 calculation with fractional entries (55.3KB, 1 page, includes linalg package function list) |
| `la1301a.pdf` | Maple output variant showing same T^7*x0 calculation with fraction display (62.3KB, 1 page, slightly different formatting from la1301.pdf) |
| `la1301b.pdf` | Maple output showing partial calculation focusing on x0 and x7 state vectors (55.6KB, 1 page, truncated view of the worksheet) |
| `la1302.pdf` | Maple output demonstrating decimal matrix approach for T^7*x0 calculation (55.1KB, 1 page, produces approximate probability values) |
| `la1302a.pdf` | Maple output variant with decimal entries showing convergence to steady state (54.8KB, 1 page, includes linalg functions list) |
| `prova.pdf` | Lecture slides on "Applications to Markov chains" from Semester 2, 2011 (443.4KB, 39 pages) covering finite Markov chain definitions, probability vectors, stochastic matrices, regular stochastic matrices, steady state vectors, with worked examples including the "Weather in the Land of Oz" problem and rat maze experiment demonstrating convergence to steady-state probability distributions |
| `la1303.graffle` | OmniGraffle diagram file (25.6KB) likely containing visual illustrations of Markov chain states, transitions, or example problem setups referenced in the lecture |

## Subdirectories

None.

## Search Tags

markov-chains math1014 linear-algebra maple computational-examples transition-matrices probability-vectors stochastic-matrices steady-state weather-oz-example semester-2-2011 scott-morrison anu lay-textbook matrix-powers state-vectors regular-stochastic eigenvalue-applications
