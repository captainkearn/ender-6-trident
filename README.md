# Ender 6 Trident Conversion

This project converts a stock Creality Ender 6 frame into a Voron Trident-style CoreXY printer.

The Ender 6 is being used as a frame donor only. Motion, Z drive, electronics, toolhead, wiring, and printed parts are treated as new conversion systems.

## Locked Baseline

- Frame: Ender 6 frame only
- Frame envelope: 495 x 495 x 650 mm
- Target build volume: 300 x 300 x 350 mm
- Bed: stock 300 x 300 mm Ender 6 bed
- Bed heater: stock heater for initial build
- Future bed heater: mains AC silicone heater with SSR and thermal fuse
- Motion: fixed-gantry CoreXY
- Gantry style: Voron Trident-inspired, inset below top frame
- X rail: MGN12H
- Y rails: MGN9H
- Belts: 2GT, 6 mm
- Toolhead: Dragon Burner
- Extruder: Orbiter 2
- Toolhead board: EBB36 Gen 2 over CAN
- Z drive: three independent Z motors
- Z hardware: three T8 leadscrews with anti-backlash nuts
- Z layout: rear-left, rear-right, front-center
- Mainboard: BTT Manta M8P
- Host: Orange Pi CM4, 4 GB RAM, 32 GB eMMC
- Firmware: Klipper

## Project Files

- `docs/00_project_spec.md`: running system specification
- `docs/01_frame_and_build_volume.md`: frame envelope, printable volume, and clearance assumptions
- `docs/02_gantry_layout.md`: CoreXY gantry layout and mount plan
- `docs/03_z_system.md`: three-point Z layout and bed support plan
- `docs/04_electronics_wiring.md`: electronics and wiring architecture
- `bom/first_pass_bom.md`: first-pass bill of materials
- `printed_parts/printed_parts_index.md`: known and planned printed parts

## Existing Source Artifacts

The workspace currently includes these printed-part archives:

- `STLS/2040 A B Drive Brackets Trident.zip`
- `STLS/2040 Front Mounts Trident..zip`

These are tracked in the printed-parts index as candidate gantry components.
