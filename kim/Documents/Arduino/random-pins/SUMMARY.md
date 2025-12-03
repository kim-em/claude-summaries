---
source_path: /Users/kim/Documents/Arduino/random-pins
generated: 2025-12-01T19:35:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# random-pins

## Overview

Arduino sketch that counts from 0 to 59048 (3^10 - 1) in base-3 (ternary), displaying the result across 10 LEDs on pins 2-11. The ternary display uses a dual-phase approach: first lighting LEDs for digits that are 1 or 2, then lighting LEDs only for digits that are 2, creating a visual distinction between the three states (off=0, dim flash=1, bright steady=2). Includes unused helper functions for binary display, cycling patterns, and random pin states.

## Key Files

| File | Purpose |
|------|---------|
| random-pins.ino | Main sketch with ternary counter display on 10 pins, plus unused binary/random/cycle functions |

## Subdirectories

No subdirectories.

## Search Tags

arduino ternary-counting base-3 led-display 10-leds pin-control counting-algorithm binary-display random-patterns cycle-patterns educational kim-morrison hardware-projects embedded-systems number-systems
