# Frame And Build Volume

## Frame Envelope

- External frame size: 495 x 495 x 650 mm
- Starting bed size: 300 x 300 mm
- Target build volume: 300 x 300 x 350 mm

## Build Volume Decision

The stock 300 x 300 mm bed is retained for the first revision. A larger bed may be possible in the Ender 6 frame, but the stock bed keeps the conversion cleaner while the gantry, Z system, and electronics are developed.

## XY Clearance Strategy

The 495 x 495 mm frame gives comfortable room around a 300 x 300 mm bed for:

- CoreXY belt paths
- Rear-mounted A/B motors
- Front idlers
- Dragon Burner toolhead clearance
- Bed wiring strain relief
- Three-point Z support
- Enclosure panel clearance

The initial mechanical target is full 300 x 300 mm printable XY. Final printable XY must be verified after toolhead offsets, rail positions, belt paths, and homing/probe choice are modeled.

## Z Clearance Strategy

The frame height is 650 mm and the target Z travel is 350 mm.

The Z design must reserve space for:

- Bottom-mounted Z motors
- Leadscrew couplers
- Bed carrier/subframe
- Bed plate, heater, magnet, and build surface
- Hotend/nozzle stack
- Fixed gantry structure
- Top panel and service clearance

## Initial Mockup Checks

Before final CAD, test these with simple blocks or printed placeholders:

- 300 x 300 bed at max-Z/top position
- Bed lowered 350 mm from print start height
- A/B motor clearance at rear
- Front idler clearance
- Cable path from moving bed to electronics bay
- CAN umbilical path from fixed frame to toolhead
