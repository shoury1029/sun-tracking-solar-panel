# Sun-Tracking Solar Panel with Automated Cleaning

**ESP32 | ESP-IDF | FreeRTOS | C | PWM | ADC | WiFi | REST API**

## Overview
Complete embedded solar tracking system built on ESP32 achieving 
~20% improvement in power delivery over static configurations.
Architected as a dedicated FreeRTOS task managing real-time sensor 
reading, motor control, and web communication concurrently.

## Features
- 12-bit ADC sampling across 3 channels - dual LDR directional 
  tracking and solar voltage monitoring
- AUTO/MANUAL dual-mode control with PWM servo and incremental 
  duty cycling for smooth positioning without overshoot
- Intelligent snow/dust detection - activates relay-driven cleaning 
  when solar output drops below 25%
- WiFi SoftAP HTTP server with 10 REST endpoints for real-time 
  monitoring and manual override
- Custom voltage regulator circuit stepping down 20V external supply

## Hardware
- ESP32 microcontroller
- LDR sensors x2
- PWM servo motor
- Relay module
- Custom voltage regulator

## Built With
- ESP-IDF framework
- FreeRTOS task architecture
- Embedded C
