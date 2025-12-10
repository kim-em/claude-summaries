---
source_path: /Users/kim/.claude/projects/-Users-kim-projects-lean-frenzymath-premises
generated: 2025-12-11T12:30:00Z
git_sha: dce44eb24f9a4be3f1c6b36d3787cea1dab9f904
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# -Users-kim-projects-lean-frenzymath-premises

## Overview

Session history for the `frenzymath-premises` project, a wrapper around the REAL-Prover's LeanSearch-PS semantic premise search system. The session documents setting up LeanSearch-PS locally for searching Lean theorems and definitions using neural embeddings and FAISS similarity search. Work included cloning REAL-Prover, understanding the LeanSearch-PS-inference server, creating a simplified setup script, and debugging deployment issues on a remote machine.

## Key Files

| File | Purpose |
|------|---------|
| 40cf3b88-5651-4fad-93d7-91d2fbc1e81d.jsonl | Single extended session (961 messages) covering LeanSearch-PS setup and development |

## Session Topics

The session covered:

1. **Initial exploration** - Reading REAL-Prover GitHub docs and understanding LeanSearch-PS-inference architecture (Flask server, FAISS index, transformer embeddings)

2. **Setup work** - Cloning REAL-Prover, installing dependencies (transformers, faiss-gpu, Flask), downloading HuggingFace models and FAISS index

3. **Script development** - Creating `leansearch-ps.py` wrapper in the `kim-em/run-leansearch-ps` GitHub repo to simplify setup

4. **Code cleanup** - Removing dead code (~53 lines) including unused `ensure_git_lfs()` function and redundant branching logic

5. **Remote deployment debugging** - Diagnosing OOM (Out of Memory) SIGKILL errors during FAISS index download on a remote machine

## Related Projects

- REAL-Prover: https://github.com/frenzymath/REAL-Prover
- User's wrapper: https://github.com/kim-em/run-leansearch-ps
- LeanSearch-PS model: https://huggingface.co/FrenzyMath/LeanSearch-PS
- FAISS index: https://huggingface.co/FrenzyMath/LeanSearch-PS-faiss

## Subdirectories

None - this is a leaf folder.

## Search Tags

leansearch-ps frenzymath real-prover lean-theorem-search premise-selection faiss neural-embeddings huggingface flask semantic-search automated-theorem-proving lean4 mathlib
