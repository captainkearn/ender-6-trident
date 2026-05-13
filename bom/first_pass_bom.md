# First-Pass BOM

This BOM is an early planning document. Quantities and lengths must be validated in CAD before ordering.

## Reused Hardware

| Qty | Item | Notes |
|---:|---|---|
| 1 | Ender 6 frame | Frame donor only |
| 1 | Stock Ender 6 300 x 300 bed | Retained for first revision |
| 1 | Stock Ender 6 bed heater | Temporary, future mains upgrade planned |

## Motion

| Qty | Item | Notes |
|---:|---|---|
| 1 | MGN12H linear rail | X axis, length TBD |
| 2 | MGN9H linear rails | Y axes, length TBD |
| 1 | 2040 extrusion, X beam | Preliminary 365-385 mm, final cut length after CAD |
| 2 | 2040 extrusions, Y rail supports | Preliminary 410-430 mm each, final cut length after CAD |
| 1 set | CoreXY idlers | 2GT, 6 mm belt path |
| 1 set | CoreXY pulleys | Match motor shaft and belt width |
| 1 spool | 2GT belt, 6 mm | Length TBD |
| 2 | NEMA 17 stepper motors | A/B motors |

## Z System

| Qty | Item | Notes |
|---:|---|---|
| 3 | NEMA 17 stepper motors | Independent Z |
| 3 | T8 leadscrews | Length TBD, likely 400-500 mm |
| 3 | T8 anti-backlash nuts | Match leadscrews |
| 3 | Leadscrew couplers | Match motor shaft and leadscrew |
| 3 | Vertical linear rails/guides | Size and length TBD |
| 1 | Bed carrier/subframe material | Aluminum plate/extrusion TBD |

## Toolhead

| Qty | Item | Notes |
|---:|---|---|
| 1 | Dragon Burner toolhead | Printed/toolhead kit |
| 1 | Orbiter 2 extruder | Direct drive |
| 1 | EBB36 Gen 2 | CAN toolhead board |
| 1 | Hotend | Model TBD |
| 1 | Probe | Type TBD |
| 1 set | Toolhead fans | Dragon Burner-specific |
| 1 set | CAN umbilical wire | 24V, GND, CANH, CANL |

## Electronics

| Qty | Item | Notes |
|---:|---|---|
| 1 | BTT Manta M8P | Main controller |
| 1 | Orange Pi CM4, 4 GB / 32 GB eMMC | Host |
| 1 | 24V PSU | Wattage TBD |
| 1 | CAN wiring/termination hardware | Exact topology TBD |
| 1 set | Ferrules/connectors | Final connector plan TBD |
| 1 set | Fans | Electronics/chamber cooling TBD |

## Future Bed Heater Upgrade

| Qty | Item | Notes |
|---:|---|---|
| 1 | 300 x 300 mains silicone heater | Future upgrade |
| 1 | SSR | Sized for heater |
| 1 | Thermal fuse | Bonded to bed |
| 1 set | AC wiring and terminals | Separate from DC wiring |
| 1 | Grounding hardware | If bed plate/heater arrangement requires it |

## Printed Parts

See `printed_parts/printed_parts_index.md`.
