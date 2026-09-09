# emonHP - Heat Pump Monitoring

**As of Aug 2026 emonHP2 hardware is not yet released**

## Introduction

_emonHP V2_ is a system for monitoring heat pump operation. It is designed to work with [OpenEnergyMonitor](https://openenergymonitor.org), but can be used as a standalone system.

The system provides the following interfaces:

- MBUS
- RS485
- Level, pulse, and OneWire inputs
- USB-C
- 40-pin Raspberry Pi header

## Getting started

### Getting a board

- Purchase a heat pump monitoring system from the [OpenEnergyMonitor Shop](https://shop.openenergymonitor.com/)
- Build your own!
  - With [KiCad](https://www.kicad.org/) installed, run `./generate.py` in the `pcb` directory (tested on Linux and macOS only) to generate manufacturing files (KiCad PCB, Gerbers, BoM).

### emonHP2

> [!NOTE]
Setting up as an integrated emonHP system requires a Raspberry Pi 4 or 5. These expose extra UART ports on the 40-pin header which are not available on older versions.

Connect the Raspberry Pi to the 40 pin header.

> [!WARNING]
Power must only be applied to one of the emonHP's USB-C port *or* the Raspberry Pi's power port, never both.

### Connections 

- DHW Status: Signal 1 input - GPIO27 - Pin 13


