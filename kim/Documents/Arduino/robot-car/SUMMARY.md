---
source_path: /Users/kim/Documents/Arduino/robot-car
generated: 2025-12-01T19:40:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 1
subdirs_count: 1
---

# robot-car

## Overview

Complete autonomous robot car Arduino project with ultrasonic obstacle avoidance capabilities. The project includes comprehensive assembly instructions (PDF) and a fully-implemented test sketch demonstrating motor control, distance sensing, and autonomous navigation. The implementation uses L298N H-bridge for dual motor control with independent PWM speed settings for differential steering, HC-SR04 ultrasonic sensor for distance measurement (using speed-of-sound calculations at 343 m/s), and a servo-controlled sensor mount that sweeps across 7 angles (60-120 degrees) to scan for obstacles. The robot executes a simple but effective autonomous behavior: continuously scanning for obstacles and backing up when any scanned angle detects objects within 200mm, otherwise driving forward with right motor compensation for straight tracking. The test-motors sketch includes an initialization motor test sequence and demonstrates enum-based motor control patterns.

## Key Files

| File | Purpose |
|------|---------|
| robot-car-instructions.pdf | Complete assembly and programming instructions for the robot car kit (25.6 MB) |

## Subdirectories

- [x] `test-motors/` - Complete motor and sensor test sketch implementing L298N H-bridge control, HC-SR04 ultrasonic distance measurement, servo-controlled 7-angle scanning, and autonomous obstacle avoidance behavior

## Search Tags

robot-car arduino obstacle-avoidance ultrasonic-sensor hc-sr04 servo-motor l298n h-bridge motor-control differential-steering pwm autonomous-robot distance-sensing sweep-scan educational-robotics kim-morrison 2023 embedded-systems
