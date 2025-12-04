---
source_path: /Users/kim/Documents/Jobs/ANU/2015/1014/Notes/Lecture24
generated: 2025-12-04T06:30:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: complete
files_count: 12
subdirs_count: 0
---

# Lecture24

## Overview

Twenty-fourth lecture materials for MATH1014 covering two major applications of linear algebra: Markov chains for text prediction/generation and Singular Value Decomposition (SVD) for image compression. The folder contains the primary lecture slides (PDF and Scribble format), a comprehensive Mathematica notebook demonstrating SVD image compression on butterfly and monarch images, Python implementations of Markov chain text generation (with Harry Potter text as corpus), and supporting visual materials including example outputs and diagrams.

## Key Files

| File | Purpose |
|------|---------|
| `MATH1014-LinearAlgebra-Lecture24.scribble.pdf` | Main lecture slides covering Markov chain text prediction (SwiftKey example, transition matrices for letter pairs) and Google PageRank algorithm using Markov chains with damping factor, plus SVD theory and image compression examples (2.9MB, 15 pages with xkcd comic, handwritten notes, and butterfly compression demonstrations) |
| `SVD-compression.nb` | Mathematica notebook implementing SVD-based image compression with practical examples on butterfly and monarch images, showing compression at different ranks (7.9MB) |
| `SVD-compression.nb.pdf` | PDF export of the Mathematica notebook for viewing without Mathematica (872KB) |
| `harry-potter.txt` | Text corpus (836KB) used as training data for Markov chain text generation examples, containing Harry Potter book text |
| `markovgen.py` | Python class implementing Markov chain text generation using word triples (2-word state, 1-word transition), with methods for building transition database from corpus and generating random text (1.2KB, 52 lines) |
| `markov.py` | Simple Python script wrapper (123 bytes) that takes filename as argument, loads corpus, and generates 100 words of Markov text using markovgen module |
| `markovgen.pyc` | Compiled Python bytecode for markovgen.py (2.0KB) |
| `markov-example.tex` | LaTeX document showing example Markov-generated Harry Potter text from GitHub project maiamcc/markovgen with humorous computer-generated quotes (1.7KB) |
| `markov-example.pdf` | Compiled PDF of markov-example.tex showing example outputs (31KB) |
| `markov-letter-at-a-time.png` | Visualization/screenshot demonstrating letter-level Markov chain text generation (222KB) |
| `swiftkey.png` | Screenshot or diagram of SwiftKey keyboard app showing predictive text functionality as real-world Markov chain application (50KB) |
| `monarch.gif` | Monarch butterfly image used as test case for SVD compression demonstration in the Mathematica notebook (49KB) |

## Subdirectories

(none)

## Search Tags

math1014 linear-algebra lecture-24 markov-chains text-generation text-prediction svd singular-value-decomposition image-compression google-pagerank python mathematica harry-potter swiftkey natural-language-processing matrix-decomposition anu 2015 scott-morrison applications
