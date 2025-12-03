---
source_path: /Users/kim/Documents/Arduino/is_it_working
generated: 2025-12-01T19:35:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# is_it_working

## Overview

Minimal Arduino diagnostic sketch for testing basic LED functionality on pin 13 (the built-in LED on most Arduino boards). The sketch blinks the LED on and off with a 1-second interval. Note: The code has a bug - pin 13 is configured as INPUT in setup() but should be OUTPUT for the digitalWrite() calls to work correctly.

## Key Files

| File | Purpose |
|------|---------|
| is_it_working.ino | LED blink test sketch - toggles pin 13 HIGH/LOW every second for basic board diagnostics |

## Subdirectories

None - this is a single-file sketch directory.

## Search Tags

arduino led-blink pin-13 diagnostic test-sketch minimal-example board-testing built-in-led debugging troubleshooting
