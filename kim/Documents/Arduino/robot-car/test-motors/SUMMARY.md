---
source_path: /Users/kim/Documents/Arduino/robot-car/test-motors
generated: 2025-12-01T19:36:00Z
git_sha: 629fb3cc99de1db687a986ca5547ddff189dce8a
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# test-motors

## Overview

Arduino test sketch for the robot car that implements the complete motor control and sensor scanning system. The code provides L298N H-bridge motor control with independent PWM speed control for differential steering, ultrasonic distance measurement using HC-SR04 sensor with speed-of-sound calculations, and servo-controlled sweeping sensor scanning across 7 angles (60-120 degrees). Includes a motor test sequence that runs on startup and a main loop implementing basic obstacle avoidance by backing up when any scanned angle detects objects within 200mm.

## Key Files

| File | Purpose |
|------|---------|
| test-motors.ino | Complete motor and sensor test sketch with enum-based motor control, ultrasonic distance reading (343 m/s sound speed calculation), and sweeping 7-angle servo scan with autonomous obstacle avoidance behavior |

## Subdirectories

None.

## Search Tags

arduino motor-control test-sketch l298n h-bridge pwm differential-steering ultrasonic-sensor hc-sr04 servo-sweep distance-measurement obstacle-avoidance enum-motor speed-calculation 343-meters-per-second 7-angle-scan autonomous-behavior robot-car kim-morrison 2023 embedded-testing
