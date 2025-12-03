---
source_path: /Users/kim/.gnupg
generated: 2025-12-01T20:30:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 8
subdirs_count: 2
---

# .gnupg

## Overview

GnuPG (GNU Privacy Guard) configuration directory managing Kim Morrison's cryptographic keys and PGP/GPG operations. The setup has migrated from GnuPG 1.x to 2.1+ (indicated by the `.gpg-v21-migrated` marker), maintaining both legacy keyrings for compatibility and the modern `private-keys-v1.d/` structure containing five private keys stored in S-expression format. The configuration connects to keyserver.kjsl.com with auto-key-retrieve enabled. Active GPG agent sockets provide cryptographic services including SSH agent emulation and smart card support. A Certificate Revocation List cache in `crls.d/` supports certificate validation. The trust database and TOFU database track key trust relationships for secure communications.

## Key Files

| File | Purpose |
|------|---------|
| `gpg.conf` | Main GnuPG configuration with keyserver settings (hkp://keyserver.kjsl.com:80), auto-key-retrieve enabled, UTF-8 charset, and no-greeting option |
| `gpg.conf.bak` | Backup copy of GnuPG configuration |
| `pubring.gpg` | Legacy public keyring (33KB) containing public keys |
| `secring.gpg` | Legacy secret keyring (8.7KB) containing private keys |
| `trustdb.gpg` | Trust database tracking key trust relationships and validity |
| `tofu.db` | Trust On First Use database (48KB) for key trust policy |
| `random_seed` | Entropy pool seed for cryptographic random number generation |
| `.gpg-v21-migrated` | Marker file indicating migration to GnuPG 2.1+ keyring format |
| `S.gpg-agent` | Unix socket for GPG agent communication |
| `S.gpg-agent.browser` | Unix socket for browser integration with GPG agent |
| `S.gpg-agent.extra` | Additional GPG agent socket |
| `S.gpg-agent.ssh` | Unix socket for SSH agent emulation via GPG |
| `S.scdaemon` | Unix socket for smart card daemon communication |

## Subdirectories

- [x] `crls.d/` - Certificate Revocation List cache directory for certificate validation (version 1 format)
- [x] `private-keys-v1.d/` - Modern GnuPG 2.1+ private key storage with 5 keys including ElGamal encryption keys

## Search Tags

gnupg gpg pgp encryption cryptography keyring keys private-keys public-keys trust-database agent sockets configuration security cryptographic-operations key-management
