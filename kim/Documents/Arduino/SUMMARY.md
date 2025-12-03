---
source_path: /Users/kim/Documents/Arduino
generated: 2025-12-01T20:45:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 0
subdirs_count: 8
---

# Arduino

## Overview

Comprehensive collection of Arduino educational projects spanning 2016-2023, demonstrating progression from basic LED control to advanced robotics. The projects showcase fundamental embedded systems concepts including digital I/O, PWM modulation, state machines, sensor integration, and motor control. Early projects (2016-2018) focus on visual displays and interactive games using LEDs, buttons, and RGB components, many based on the SparkFun Inventor's Kit curriculum. The collection culminates in a sophisticated autonomous robot car (2023) featuring ultrasonic obstacle avoidance, servo-controlled scanning, and H-bridge motor control. Projects demonstrate both theoretical understanding (binary/ternary counting systems, positional notation) and practical hardware skills (debouncing, edge detection, sensor fusion). The work reflects hands-on learning with increasing complexity over time, from simple diagnostic sketches to multi-component autonomous systems.

## Key Files

No files directly in this directory - all content is organized into project subdirectories.

## Subdirectories

- [x] `_20160212-push-button-game/` - Two-player competitive game using buttons to flip RGB LED color and light team LED strips, demonstrates turn-based state machine logic (2016)
- [x] `_20180428-counting-in-binary/` - Configurable base-n counter (default base-10) displaying numbers on 8 LEDs using positional notation with PWM brightness modulation, features recursive digit decomposition algorithm (SparkFun Inventor's Kit Circuit #4, 2018)
- [x] `colour-fade/` - RGB LED color mixing with smooth linear interpolation transitions through custom color sequence (cyan → chartreuse → dark violet → crimson), customized from SparkFun tutorial
- [x] `is_it_working/` - Minimal diagnostic sketch for testing LED on pin 13, contains instructive pinMode bug (INPUT instead of OUTPUT)
- [x] `libraries/` - Standard Arduino libraries directory placeholder with installation reference, no libraries currently installed
- [x] `push-buttons/` - Dual-button LED toggle demonstrating proper edge detection and debouncing techniques using state tracking for falling edge identification (February 2016)
- [x] `random-pins/` - Ternary (base-3) counter displaying 0-59048 across 10 LEDs with dual-phase visualization (dim flash for 1, bright steady for 2), includes unused helper functions for binary/random patterns
- [x] `robot-car/` - Autonomous robot with L298N H-bridge motor control, HC-SR04 ultrasonic distance sensing, servo-controlled 7-angle scanning (60-120°), differential steering with PWM speed control, and obstacle avoidance behavior (backs up when objects detected within 200mm), includes comprehensive assembly instructions PDF (25.6MB, 2023)

## Search Tags

arduino microcontroller embedded-systems educational-projects led-control rgb-led pwm-modulation analog-write digital-input digital-output push-buttons edge-detection debouncing state-machine turn-based-logic binary-counter ternary-counter base-n-counting positional-notation number-visualization recursive-algorithm color-mixing linear-interpolation color-fading robot-car autonomous-robot obstacle-avoidance ultrasonic-sensor hc-sr04 servo-motor l298n h-bridge motor-control differential-steering distance-sensing sweep-scan sparkfun-inventors-kit hardware-projects electronics-prototyping kim-morrison 2016 2018 2023
