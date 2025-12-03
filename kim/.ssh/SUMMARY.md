---
source_path: /Users/kim/.ssh
generated: 2025-12-01T19:30:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 27
subdirs_count: 1
---

# .ssh

## Overview

SSH configuration directory managing authentication and access to a diverse ecosystem of development environments and computational resources. The directory contains 27 key files spanning nearly a decade (2017-2025), organized around several key environments: GitHub (both standard and HoTT project), CMU's Hoskinson cluster (10 nodes), personal Lean-FRO servers (chonk, chonk2), personal machines (carica, idaeus, edulis, arguta), AWS EC2 infrastructure, academic computational resources (NCI, GAN, MSRI, DOI), and historical Bitbucket access. The configuration includes a dedicated subdirectory (`code_gitpod.d/`) for Gitpod cloud workspace integration with VS Code, featuring auto-managed proxy settings. The main `config` file orchestrates connections via GitHub's HTTPS fallback (port 443), complex proxy chains, and host-specific settings optimized for both production work and historical academic collaborations.

## Key Files

| File | Purpose |
|------|---------|
| `config` | Main SSH configuration with Gitpod integration, GitHub over HTTPS (port 443), CMU Hoskinson cluster hosts (0-9), local machines (idaeus, edulis, arguta, carica), chonk servers, EC2, and a complex zigzag proxy chain |
| `known_hosts` | SSH known hosts database (19KB, current) |
| `known_hosts.old` | Previous version of known hosts (18KB, backup) |
| `authorized_keys` | Two authorized public keys for remote SSH access (from Scott@Wesley and gan.anu.edu.au) |
| `id_rsa` | Default RSA private key |
| `id_rsa.pub` | Default RSA public key |
| `id_ed25519_new` | Ed25519 private key (created November 19, 2025) |
| `id_ed25519_new.pub` | Ed25519 public key (created November 19, 2025) |
| `chonk` | Private key for chonk.lean-fro.org and chonk2.lean-fro.org servers (created April 3, 2025) |
| `chonk.pub` | Public key for chonk servers |
| `aws-2025-05-17.pem` | AWS EC2 PEM key file (created May 17, 2025) |
| `github_rsa` | GitHub-specific RSA key pair |
| `github_rsa.pub` | GitHub RSA public key |
| `github-hott-2017` | GitHub key for HoTT project from 2017 |
| `github-hott-2017.pub` | GitHub HoTT public key from 2017 |
| `scottmorrison_Bitbucket` | Bitbucket key pair for scottmorrison account |
| `scottmorrison_Bitbucket.pub` | Bitbucket public key |
| `id_rsa.nci` | NCI (National Computational Infrastructure) specific RSA key |
| `id_rsa.nci.pub` | NCI RSA public key |
| `id_rsa.gan` | GAN (gan.anu.edu.au) specific RSA key |
| `id_rsa.gan.pub` | GAN RSA public key |
| `20170614-msri-791` | MSRI (Mathematical Sciences Research Institute) key from June 14, 2017 |
| `20170614-msri-791.pub` | MSRI public key from 2017 |
| `doi-direct` | DOI direct access key pair |
| `doi-direct.pub` | DOI direct public key |
| `math-private-key.ppk` | PuTTY format private key for math server |

## Subdirectories

- [x] `code_gitpod.d/` - Gitpod-managed SSH configuration for automatic VS Code integration with cloud workspaces via custom proxy (complete)

## Search Tags

ssh ssh-keys authentication remote-access github aws ec2 cmu hoskinson lean-fro chonk gitpod configuration private-keys public-keys known-hosts authorized-keys rsa ed25519 bitbucket nci gan msri doi security credentials
