# Next steps

## Housing

To get the classic look, the camera goes inside an outdoor-style housing with a sun shield. The Samsung SHB-4200 is the style I like. Generic "CCTV outdoor housing with sunshield" listings look almost the same and cost $20-40.

Before buying: measure the camera with the lens on, then check the housing's inside length. A heater ("H") version isn't needed indoors.

## Capturing the feed

To record or view the camera from my phone instead of only on the CRT:

1. A USB composite capture stick (about $15). The UTV007 chip works with Linux's built-in usbtv driver.
2. Plug it into my always-on mini PC.
3. Use ffmpeg (or go2rtc) to turn the feed into a stream, reachable over Tailscale.
4. Optional: burn in a "CAM 01" timestamp overlay with ffmpeg's drawtext filter, for the classic security-tape look.

## Night vision

The TK-C750U has no IR. A cheap 850 nm IR illuminator would light the room in the dark, but this is a color camera and its IR response isn't known yet. Test before buying.

## Pan and tilt (maybe later)

Moving the camera from a keyboard or gamepad would need:

- A motorized pan-tilt head with a built-in Pelco-D / RS-485 receiver
- A USB-to-RS-485 adapter
- A small web page that reads the gamepad in the browser and sends Pelco-D commands

A used all-in-one analog PTZ camera, which has the motor, zoom and control board in one unit like in the SimonRetro video in the references, might cost less than buying a pan-tilt head separately.
