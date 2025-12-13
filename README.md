# wire-rack-mounter
A system of 3d-printable designs for mounting things to wire rack shelving units.

These are spreadsheet-parametric designs in FreeCAD, you can edit the spreadsheet values to change the geometry for your needs.

I typically print these in PETG for strength, but PLA can work for lighter applications.


## Wire Rack Pole Mounting System
**External hardware required: M3x0.5 hex nuts and screws (minimum 8mm threaded length)**

These are designed to clamp onto the poles of the shelving units.

The basic unit is the PoleMounterSingle, of which two identical copies are needed.
One side has 2x M3x0.5 hex nut inserted into it, while the other has screws into those nuts.
Screws are 20mm apart and must have a minimum length of ~8mm, but can be longer.

PoleMounterSingle is the smallest one and is also used with other designs as the back clamping side.

Variations include:
- Note: these link the geometry from **PoleMounterBase** and re-use its parameters.
- **PoleMounterSingle** has a slot on the other side that takes a hex nut, which a screw can be screwed into.
  The screw creates a stud, which an object with a keyhole hanger can be attached to.
  - Note, nominal dimensions for screw hexes:
    - M3: normal fit clearance 3.45mm, W 5.5mm, D 2.4mm
    - M4: normal fit clearance 4.5mm, W 7.0mm, D 3.2mm
- **PoleMounterTall** the tall version of the above, allowing vertical flexibility in where the screw goes.
  Typically one mounting point is fixed to the pole rib with PoleMounterSingle, while the other one uses PoleMounterTall to match the mounting hole to a non-rib location.
- **PoleMounterHook** has a hook.
- **PoleMounterAP303H** mounts an Aruba AP-303H access point using the keyhole slot.

These designs follow and older architecture and eventually will be cleaned up - but should be compatible with the above.
- **WireRackMounterPerpendicularPole** has a hole to mount a smaller pole perpendicularly to the main shelving unit pole. This can be used to, for example, mount lights or other devices offset from the main pole.
  - This is designed to work with a system of 10mm poles. These are commonly part of systems with M8 threads and include mating goosenecks.
  - This object has two bodies, the main mount and a pad. The pad clamps the smaller pole, with clamping tension from screws.


## Other Pole Mounters
- **ElfaDrawerPoleMounter** attaches to a rectangular profile pole and clamps to the pole with a ~10mm M3 screw.
  It is sized for Elfa drawers and should attach to either the vertical poles or the horizontal cross bars (roughly 10x20mm profile).

## Adapters
- **HexNutAdapter** is a parameterized nut adapter that adapts a metal M2 nut into a 3d printed M3 nut.
  This allows use of M2 nuts and screws in the pole mounter sized for M3.
  - Dimensions are critical, and as-is, this barely prints on a 0.4mm nozzle and is a snug fit into the pole mounter.
    If a brim is needed, I've found a brim separation gap helps make removing the brim cleanly easier. I've had good luck with 0.4mm gap.
- **GeekwormP579** screws into the M3 PoleMounter and presents a keyhole head for the Geekworm P579 series Raspberry Pi 5 bases.