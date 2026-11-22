# Power and wiring

## Picking a 24 V AC supply

The camera needs **24 V AC**. The mistake I almost made was buying an "AC/DC adapter." That phrase means AC in from the wall and **DC out**, which is wrong for this camera.

How to tell them apart:

- Read the **output** line on the label or in the listing. You want **"Output: 24V AC"** or **"24V ~"** (wavy line).
- **"Output: 24V DC"** or the DC symbol (a solid line over a dashed line) is wrong.
- Listings that say **"transformer"** are usually AC. **"Switching power supply"** and **"AC/DC adapter"** are usually DC.
- **Doorbell and thermostat transformers** (Ring, Nest, "C-wire adapter") are always 24 V AC, cheap, and often come with a long cable ending in bare wires. That's what I bought.

Rating: the camera draws 3.3 W, so anything from 500 mA (12 VA) to 40 VA is more than enough.

## First power-on

With the transformer **unplugged**:

1. Look the camera over. Check for loose parts, rattles, and corrosion on the terminals.
2. Set the DIP switches to the starting settings in [jvc-tk-c750u.md](jvc-tk-c750u.md).
3. Loosen the screws on terminals 1 and 2.
4. Wrap one bare wire clockwise under each screw and tighten. Either wire can go in either terminal.
5. Make sure no stray copper strands bridge the two terminals.
6. Connect the BNC end of the video cable to VIDEO OUT and the RCA end to the TV's yellow video input.
7. Switch the TV to its AV / Video input.
8. Plug in the transformer. The green POWER LED should light up.
9. Open the lens iris, zoom wide (2.8 mm), and focus until the picture is sharp.

## Troubleshooting

**No POWER light**

- Check the transformer outlet with something else
- Check that both wires are clamped under the screws, on metal and not insulation
- Measure the transformer's output with a multimeter set to AC volts. It should read about 24-28 V with no load

**Power light on, but a blank or blue screen**

- Make sure the TV is on the right input
- Reseat the BNC connector (push and twist to lock it)
- Try the second cable from the 2-pack
- Check that the lens cap is off and the iris isn't closed

**Picture is all white or all black**

- Check that the auto-iris cable is plugged into the camera
- Try toggling AES

**Picture rolls or flickers**

- Set sync to INT
- If using LL, adjust PHASE

**Colors look wrong**

- Use ATW, or point at something white and press SET in AWB mode

**Soft focus that won't sharpen**

- Adjust back focus: loosen BF LOCK, slide the mount until it's sharp at both ends of the zoom range, then tighten

**Black and white only**

- On a TV set to the wrong standard, an NTSC signal can show up without color. Make sure the TV is set to NTSC (or Auto).

## Safety

The transformer is a sealed, UL-listed Class 2 plug-in supply. The 120 V side never leaves the brick. Even so, wire everything with it unplugged, and don't leave bare wire ends exposed.
