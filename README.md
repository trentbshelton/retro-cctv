# retro-cctv

I'm learning how old analog CCTV cameras work by buying one, wiring it up myself, and getting a live picture on a CRT TV. No network, no app, no cloud. Just a camera, a power supply, and a coax cable going to a screen.

I got the idea from a video of someone powering up an old security camera with no documentation and figuring it out. I wanted to do the same thing and understand the hardware, not just plug in a Wi-Fi camera.

## Status

- [x] Researched analog vs. HD-over-coax vs. IP cameras
- [x] Compared cameras and picked one
- [x] Bought the camera (JVC TK-C750U with a 2.8-12 mm lens and wall bracket)
- [x] Bought a 24 V AC power transformer and BNC-to-RCA cables
- [ ] Camera arrives, inspect it, power it on
- [ ] Get a picture on the CRT
- [ ] Tune the settings (white balance, backlight, focus, line lock)
- [ ] Put it in an outdoor-style housing with a sun shield
- [ ] Capture the feed on a computer and view it from my phone

## Parts

| Part | Price |
|---|---|
| JVC TK-C750U color box camera, 2.8-12 mm CS varifocal auto-iris lens, wall bracket (used, untested, eBay) | $28 + shipping and tax ($38.99 total) |
| 24 V AC plug-in transformer with bare-wire leads (doorbell / thermostat type) | about $12 |
| BNC-to-RCA cables, 3 ft, 2-pack | $5.98 |
| Total so far | about $57 |

## How it hooks up

```
 wall outlet
     |
 24 V AC transformer
     |  (2 bare wires, either order)
     v
 +---------------------+          BNC -> RCA cable          +-----------+
 |  JVC TK-C750U       |  VIDEO OUT ----------------------> | CRT TV    |
 |  terminals 1 and 2  |                                    | yellow AV |
 +---------------------+                                    +-----------+
```

## Docs

- [How analog CCTV works](docs/how-analog-cctv-works.md): camera types, power, video signal, lenses, NTSC vs. PAL
- [Choosing a camera](docs/choosing-a-camera.md): what I looked at, what I almost bought, and why I picked the JVC
- [JVC TK-C750U reference](docs/jvc-tk-c750u.md): what every switch and terminal on the back does
- [Power and wiring](docs/power-and-wiring.md): picking a power supply (and the AC vs. DC trap), first power-on steps, troubleshooting
- [Next steps](docs/next-steps.md): housing, capturing the feed, maybe pan/tilt later
- [References](docs/references.md)

I used AI for some guidance with the research and with picking parts.
