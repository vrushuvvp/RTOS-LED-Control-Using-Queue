# ESP32 FreeRTOS Queue-Based LED Controller

This project demonstrates event-driven multitasking using FreeRTOS on ESP32.
Instead of shared variables and mutexes, inter-task communication is implemented
using queues to avoid race conditions and improve responsiveness.

## Architecture
- Button Task: Detects button press and sends event to queue
- LED Task: Waits on queue and updates LED state
- RTOS handles scheduling and task switching

## Why Queues?
- Avoids shared memory
- Prevents race conditions
- Event-driven design
- Scales better than mutex-based approach

## Concepts Used
- FreeRTOS Tasks
- FreeRTOS Queues
- Task Priorities
- Blocking vs Polling
- Embedded Concurrency Design

## Hardware
- ESP32
- Push Button
- LED

## Key Learning
This project focuses on software architecture and synchronization,
not just GPIO control.
