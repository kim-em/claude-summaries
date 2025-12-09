---
source_path: /Users/kim/.claude/skills/whatsapp
generated: 2025-12-09T10:20:00Z
git_sha: d3c5486ba8cc6e05ec408002550fd039e067c322
git_branch: master
status: complete
files_count: 12
subdirs_count: 0
---

# whatsapp

## Overview

WhatsApp messaging skill using the Baileys library (unofficial WhatsApp Web API) for both sending and reading messages. Provides authentication via QR code scanning, message sending, and multiple message reading strategies: real-time monitoring (read.js), history fetch from WhatsApp (read-history.js), and querying locally stored messages (query.js). Includes a background logger (logger.js) that runs as a launchd service on carica, storing all messages to ~/projects/corpus/whatsapp-messages.json for persistent searchable history. The skill is intentionally against WhatsApp's ToS but noted as low risk for personal/low-volume use.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Comprehensive skill documentation covering setup, sending, and three reading workflows (query stored, monitor real-time, fetch history); explains launchd automation and corpus integration |
| auth.js | Authentication script that displays QR code for linking WhatsApp device; saves session credentials to auth_info/ directory |
| send.js | Message sending script with clean output (suppresses Baileys logging); takes phone number and message as command-line arguments |
| logger.js | Background message logger that connects to WhatsApp and stores all incoming/outgoing messages to JSON file; designed to run continuously via launchd |
| query.js | Query tool for searching stored messages by phone number or text match; searches local message history collected by logger (deprecated in favor of ~/projects/corpus/whatsapp-query.js) |
| read.js | Real-time message monitor that watches for new messages from a specific contact; displays messages as they arrive |
| read-history.js | Attempts to fetch historical messages from WhatsApp servers; limited by WhatsApp Web API restrictions on history access |
| com.whatsapp.logger.plist | Launchd configuration for auto-starting logger.js on boot on carica machine; stores output to ~/projects/corpus/whatsapp-logger.log |
| package.json | Node dependencies: @whiskeysockets/baileys, pino (logging), qrcode-terminal; configured as ESM module |
| package-lock.json | Locked npm dependencies for reproducible installs |
| test | Bash test script with unit tests (dependency checks, syntax validation) and E2E test (sends message to self) |
| .gitignore | Excludes node_modules/, auth_info/ (session credentials) from version control |

## Subdirectories

No subdirectories.

## Search Tags

whatsapp messaging baileys qr-code authentication nodejs esm api unofficial skill send-message read-messages phone-number test-suite e2e-test credentials session-management logger background-service launchd query real-time-monitoring history-fetch corpus persistent-storage output-suppression
