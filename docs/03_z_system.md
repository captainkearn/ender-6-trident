# Z System

## Baseline

- Z architecture: Trident-style moving bed
- Z motors: three independent NEMA 17 motors
- Z drive: three vertical T8 leadscrews
- Z nuts: anti-backlash T8 nuts
- Layout: rear-left, rear-right, front-center
- Bed leveling: Klipper `Z_TILT_ADJUST`
- Target Z travel: 350 mm

## Layout

The bed should be supported at three points:

- Rear-left Z point
- Rear-right Z point
- Front-center Z point

The bed carrier should use a three-point support pattern so the Z motors can tram the bed without fighting a four-point constrained plate.

## Recommended Hardware

- 3x NEMA 17 Z motors
- 3x T8 leadscrews, likely 8 mm lead
- 3x anti-backlash T8 nuts
- 3x motor-to-leadscrew couplers
- 3x vertical linear guides, likely MGN12H or MGN9H
- 1x rigid bed carrier/subframe
- 3x bed mount points with adjustment/thermal isolation as needed

## Leadscrew Length

First-pass expected leadscrew length: 400-500 mm.

Final length depends on:

- Z motor mounting height
- Coupler height
- Bed carrier thickness
- Bed start height near nozzle
- Required 350 mm travel
- Safe overtravel margin

## Bed Carrier Notes

The stock 300 x 300 bed should mount to a new rigid carrier rather than rely on the original Ender 6 bed support. The carrier should:

- Support the bed at three controlled points
- Keep the bed plane stiff
- Include bed wiring strain relief
- Leave room for a future mains heater thermal fuse
- Avoid overconstraining the bed plate as it expands

## Klipper Planning

The final Klipper config should define:

- `stepper_z`
- `stepper_z1`
- `stepper_z2`
- `z_tilt`
- Probe configuration
- Bed mesh configuration

Probe choice is still open and should be selected before final toolhead wiring and config.
