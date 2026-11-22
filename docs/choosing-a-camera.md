# Choosing a camera

## What I wanted

- The classic analog security-camera look, not a modern Wi-Fi camera
- A box camera, the kind that goes inside a housing with a sun shield
- Cheap enough to experiment with
- Works on a US TV (NTSC)

## Analog or IP?

I first considered a used IP box camera recording to Frigate on my home server. That's the better choice if the goal is actually watching a room from my phone. I picked analog instead because I wanted the retro picture and wanted to learn the hardware from the ground up. I can still capture the analog feed onto a computer later (see [next-steps.md](next-steps.md)).

## Cameras I looked at

**JVC TK-C8301RU** (around 2012, open box, $129.99)

- Built-in 2.8-10.5 mm lens and 12 IR LEDs, 600 TVL, runs on 12 V DC or 24 V AC
- Clean enough to use without a housing, with night vision
- It's the nicest option, but it's the most expensive. Few box cameras have both a built-in lens and IR, which is why it costs more.

**Samsung SCB-3000N** (used, around $50)

- 600 TVL day/night box camera, 12 V DC or 24 V AC
- Made to fit the Samsung SHB-4200 housing, which is the look I wanted
- Doesn't come with a lens, so add $15-25 for a CS-mount lens

**Sony SSC-C104 Hyper HAD** (used, $36 or best offer)

- Made in Japan, with the lens included and the power wires already attached
- 24 V AC only, and the lens's focal length wasn't listed

**JVC TK-C750U** (used, untested, $34.99 or best offer)

- Late-90s JVC color camera, US/NTSC version
- Came out of a store install. The seller said it worked when it was taken down.
- Comes with a 2.8-12 mm f/1.4 CS varifocal auto-iris lens and a wall bracket
- 24 V AC only, no IR, sold as-is with no returns

I skipped domes and bullets (I wanted the box look), HD-over-coax cameras (they won't work on a TV), and anything PAL.

## What I picked

**JVC TK-C750U, for $28 with an accepted offer.**

The Sony and the JVC cost about the same and both run on 24 V AC, but the JVC listing showed a wide 2.8-12 mm zoom lens and a mount. Wide is what I need for a room. The untested, no-returns part is a risk, but at $28 it's a cheap one.

## Getting over the 24 V AC worry

At first I wanted to avoid 24 V AC because a "transformer" sounded dangerous. It turns out to be just a sealed plug-in brick like a phone charger. The 120 V from the wall stays inside, and only 24 V comes out, the same as a doorbell or thermostat. Once I understood that, being 24 V AC only stopped being a dealbreaker.

## Things I dropped (for now)

- **Pan and tilt from a gamepad.** That would need a motorized pan-tilt head with a Pelco-D (RS-485) receiver, a USB-to-RS-485 adapter, and a control page. It roughly doubled the cost, so I'm starting with the basics. See [next-steps.md](next-steps.md).
