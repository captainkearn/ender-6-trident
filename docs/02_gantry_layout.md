# Gantry Layout

## Baseline

- Motion type: CoreXY
- Gantry style: fixed-height Voron Trident-inspired gantry
- Mounting style: inset below the top frame
- X rail: MGN12H
- Y rails: MGN9H
- Belts: 2GT, 6 mm
- A/B motors: rear-mounted NEMA 17
- Toolhead: Dragon Burner with Orbiter 2 and EBB36 Gen 2

## Gantry Assemblies

The first-pass gantry is split into these assemblies:

| Assembly | Purpose |
|---|---|
| Rear A/B motor mounts | Hold CoreXY drive motors and rear belt path |
| Front idler mounts | Hold front idlers and close the belt loop |
| Y rail mounts | Support left and right MGN9H rails |
| X beam | Carries MGN12H rail and toolhead carriage |
| XY joints | Connect X beam to Y carriages |
| Toolhead carriage | Dragon Burner-compatible carriage on MGN12H |

## 2040 Extrusion Plan

The current candidate STL set is intended for 2040 extrusion. The gantry BOM should therefore assume 2040 for the main gantry structure unless the CAD fit check proves otherwise.

First-pass extrusion assumptions:

| Position | Extrusion | Preliminary length | Notes |
|---|---:|---:|---|
| Left Y rail support | 2040 | 410-430 mm | Final length depends on front/rear mount stack and inner frame depth |
| Right Y rail support | 2040 | 410-430 mm | Match left side |
| X beam | 2040 | 365-385 mm | Must support 300 mm X travel plus MGN12H carriage clearance |

These are planning lengths, not cut lengths. Final lengths should be set from the measured internal frame opening and the exact printed mount offsets.

## Existing Candidate Parts

The workspace already includes candidate gantry parts:

| Archive | Contents |
|---|---|
| `STLS/2040 A B Drive Brackets Trident.zip` | `A_Lower_Final V1.STL`, `A_Upper_Final V1.STL`, `BLower modified.STL`, `BUpper modified.STL` |
| `STLS/2040 Front Mounts Trident..zip` | `Stepper Left.STL`, `Stepper Right.STL` |

These parts should be treated as candidate hardware until fit is checked against the Ender 6 frame and chosen belt path.

## Mounting Concept

The gantry should sit just below the top cube of the Ender 6 frame. This preserves Z height while leaving room for:

- Top panel clearance
- Belt service access
- A/B motor wiring
- CAN umbilical routing
- Lighting or chamber accessories

The gantry mounts should reference the vertical frame extrusions and top frame structure. Avoid relying only on printed parts in bending where a metal extrusion or direct rail support can carry the load.

## Rail Length Targets

Final rail lengths require measurement and CAD validation, but the first-pass expectation is:

- X MGN12 rail: approximately 350-380 mm range
- Y MGN9 rails: approximately 380-420 mm range

The chosen rail lengths must allow full 300 mm travel plus carriage length, end clearance, and belt/idler clearance.

## CAD Checks Required

- Toolhead reaches all four corners of 300 x 300 bed
- Dragon Burner fan ducts clear front frame and bed clips, if used
- A/B motors clear rear frame and panels
- Belt path is coplanar and does not rub printed mounts
- X beam does not collide with front idler mounts
- Toolhead umbilical has a clean path at all XY positions
