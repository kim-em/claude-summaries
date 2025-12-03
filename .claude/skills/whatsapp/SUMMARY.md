---
source_path: /Users/kim/.claude/skills/whatsapp
generated: 2025-12-01T13:30:00Z
git_sha: b75fd51d2702e678b15ef7ce28cf6993a31edb62
git_branch: master
status: complete
files_count: 8
subdirs_count: 0
---

# whatsapp

## Overview

WhatsApp messaging skill using the Baileys library (unofficial WhatsApp Web API) for sending messages programmatically. Provides authentication via QR code scanning and message sending functionality. Includes a comprehensive test suite that validates dependencies, syntax, and can perform end-to-end message testing. The skill is intentionally simple (send-only, no message reading) and acknowledges being against WhatsApp's ToS while noting low risk for personal/low-volume use.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill documentation with setup instructions, usage examples, and phone number formatting |
| auth.js | Authentication script that displays QR code for linking WhatsApp device; saves session to auth_info/ |
| send.js | Message sending script with clean output (suppresses Baileys logging); takes phone number and message as args |
| package.json | Node dependencies: @whiskeysockets/baileys, pino (logging), qrcode-terminal; configured as ESM module |
| package-lock.json | Locked npm dependencies for reproducible installs |
| test | Bash test script with unit tests (dependency checks, syntax validation) and E2E test (sends message to self) |
| .gitignore | Excludes node_modules/ and auth_info/ (session credentials) from version control |

## Subdirectories

No subdirectories.

## Search Tags

whatsapp messaging baileys qr-code authentication nodejs esm api unofficial skill send-message phone-number test-suite e2e-test credentials session-management output-suppression
