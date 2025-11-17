# wire-rack-mounter
A system of 3d-printable designs for mounting things to wire rack shelving units.

These are spreadsheet-parametric designs in FreeCAD, you can edit the spreadsheet values to change the geometry for your needs.

I typically print these in PETG for strength, but PLA can work for lighter applications.


## Pole Mounting System
**External hardware required: M3x0.5 hex nuts and screws (minimum 8mm threaded length)**

These are designed to clamp onto the poles of the shelving units.

The basic unit is the WireRackMounterSingle, of which two identical copies are needed.
One side has 2x M3x0.5 hex nut inserted into it, while the other has screws into those nuts.
Screws must have a minimum length of 8mm, but can be longer.

WireRackMounterSingle is the smallest one and is also used with other designs as the back clamping side.

New Aruba
- Heatsink fin height 9.16
- KEyhole total depth 4.30mm thickness ~2.0mm
70mm BSC
8.1mm OD  5.38mm ID
appriox 5mm offset height to avoid ethernet

All variations include:
- **WireRackMounterSingle** has a slot on the other side that takes a nex nut, which a screw can be screwed into.
The screw creates a stud, which an object with a keyhole hanger can be attached to.
  - Note, nominal dimensions for screw hexes:
    - M3: normal fit clearance 3.45mm, W 6.0mm, D 2.4mm
    - M4: normal fit clearance 4.5mm, W 7.0mm, D 3.2mm
- **WireRackMounterPerpendicularPole** has a hole to mount a smaller pole perpendicularly to the main shelving unit pole. This can be used to, for example, mount lights or other devices offset from the main pole.
  - This is designed to work with a system of 10mm poles. These are commonly part of systems with M8 threads and include mating goosenecks.
  - This object has two bodies, the main mount and a pad. The pad clamps the smaller pole, with clamping tension from screws.
- **WireRackMounterHook** mounts a hook.
- **WireRackMounterAP303H** mounts an Aruba AP-303H access point.
