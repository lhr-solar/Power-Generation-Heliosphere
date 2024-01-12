# ORDERING AND ASSEMBLY

## Ordering

- Generate gerbers using JLC PCB fabrication toolkit (1 button click).
- Navigate to JLCPCB site and upload zip file provided.
- No assembly is performed for this PCB. Order as default FR4, 2 layer.

## Assembly

Use the ibom.html provided in the outputs file for placement.

- Solder R101 to PCB.
  - Solder one side before other. Keep package flat against PCB.
- Solder D106 to PCB.
  - Marking side is the cathode (positive). Solder closest to enclosed line on silkscreen.
  - Solder one side before other. Keep package flat against PCB.
- Solder VR101 - VR105 to PCB.
  - Place on PCB, hold, flip PCB, bend legs outwards to keep in place.
- Solder D101 - D105 to PCB.
  - Tin surfaces of pads, both on PCB and LED package. Keep flat.
  - Use masking tape to hold package to bottom side, facing down. Align with silkscreen.
  - With a soldering iron, solder from top of PCB into holes. Make sure
    soldering tip can reach the package. Hold firm to each other. Fill hole with
    solder. Hold long enough that solder wicks down to PCB pad. A negative
    indent is good.
  - Verify that the pieces are soldered down properly and flush. Gaps require
    resoldering and will likely not light up during testing.
- Solder AWG 18 wires to positive, negative contacts indicated on silkscreen.