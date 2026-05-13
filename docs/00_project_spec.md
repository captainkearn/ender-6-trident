# Project Spec

## Goal

Convert a Creality Ender 6 frame into a Voron Trident-style enclosed CoreXY printer.

The Ender 6 contributes the frame only. All motion, Z drive, electronics, toolhead, and wiring are new or conversion-specific systems.

## Coordinate Assumptions

- X axis: left to right when facing the printer
- Y axis: front to back
- Z axis: bed moves down as print height increases
- Origin strategy: to be finalized with gantry/toolhead CAD

## Locked Decisions

| System | Decision |
|---|---|
| Frame | Stock Ender 6 frame only |
| Frame size | 495 x 495 x 650 mm |
| Build volume target | 300 x 300 x 350 mm |
| Bed plate | Stock 300 x 300 mm Ender 6 bed |
| Initial bed heater | Stock Ender 6 bed heater |
| Future bed heater | Mains AC silicone heater, SSR, thermal fuse |
| Motion system | CoreXY |
| Gantry | Fixed-height, Trident-style, inset below top frame |
| X rail | MGN12H |
| Y rails | MGN9H |
| Belts | 2GT, 6 mm |
| A/B motors | Rear-mounted NEMA 17 |
| Toolhead | Dragon Burner |
| Extruder | Orbiter 2 |
| Toolhead board | EBB36 Gen 2 over CAN |
| Mainboard | BTT Manta M8P |
| Host | Orange Pi CM4, 4 GB RAM, 32 GB eMMC |
| Firmware | Klipper |
| Z motors | Three independent NEMA 17 motors |
| Z drive | Three vertical T8 leadscrews |
| Z nuts | Anti-backlash T8 nuts |
| Z layout | Rear-left, rear-right, front-center |

## Open Measurements

These measurements should be captured before CAD is finalized:

- Exact inner X clearance between vertical frame members
- Exact inner Y clearance between vertical frame members
- Top frame extrusion profile and usable mounting faces
- Existing bottom frame clearance for Z motors and leadscrew couplers
- Bed plate thickness and stock heater wiring exit location
- Available rear clearance for A/B motors and belt path
- Panel thickness and panel mounting offsets, if enclosure panels are retained

## Design Priorities

1. Preserve the 300 x 300 mm XY target without pushing toolhead clearance to the edge.
2. Keep the 350 mm Z target realistic after bed carrier, motor, coupler, nozzle, and gantry clearance.
3. Use serviceable assemblies: gantry, bed/Z, electronics, and toolhead should be removable without full frame teardown.
4. Leave a migration path from the stock DC bed heater to a future mains heater.
5. Prefer proven Voron-compatible hardware where it fits the Ender 6 frame.
