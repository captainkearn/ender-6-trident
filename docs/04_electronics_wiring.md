# Electronics And Wiring

## Baseline Electronics

- Mainboard: BTT Manta M8P
- Host: Orange Pi CM4, 4 GB RAM, 32 GB eMMC
- Toolhead board: EBB36 Gen 2
- Toolhead link: CAN
- Firmware: Klipper
- Power system: 24V DC for initial build

## Mainboard Responsibilities

The Manta M8P handles:

- A motor
- B motor
- Z0 motor
- Z1 motor
- Z2 motor
- Stock bed heater control
- Bed thermistor
- Chamber/case fans
- Lighting, if added
- CAN connection to EBB36

## EBB36 Responsibilities

The EBB36 Gen 2 handles:

- Orbiter 2 extruder motor
- Hotend heater
- Hotend thermistor
- Hotend fan
- Part cooling fan
- Probe input, depending probe choice
- Toolhead accelerometer

## Initial Bed Heater

The stock Ender 6 bed heater is retained for the initial build.

Before wiring, confirm:

- Bed heater voltage
- Bed heater wattage/current
- Bed thermistor type
- Wire gauge and connector condition
- Manta M8P bed output suitability

## Future Mains Bed Heater

Design space should be reserved for:

- SSR
- AC input routing
- Thermal fuse mounted to bed
- Earth/ground bonding where applicable
- Separated AC and DC wire paths
- Strain relief for moving bed wiring

## Wiring Architecture

```text
24V PSU
|-- Manta M8P
|   |-- A/B motors
|   |-- Z0/Z1/Z2 motors
|   |-- stock DC bed heater
|   |-- bed thermistor
|   |-- chamber/case fans
|   `-- CAN + 24V/GND to EBB36
|
`-- auxiliary loads as needed

EBB36 Gen 2
|-- Orbiter 2
|-- hotend heater
|-- hotend thermistor
|-- toolhead fans
|-- probe
`-- accelerometer
```

## Open Electrical Decisions

- Probe type
- Hotend model
- PSU rating
- Chamber fan/filter choice
- Exhaust fan choice
- Lighting type and voltage
- Emergency stop or front power switch arrangement
