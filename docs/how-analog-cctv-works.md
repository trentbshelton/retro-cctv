# How analog CCTV works

CCTV means closed-circuit television. The video goes over a cable straight from the camera to a monitor or recorder. It isn't broadcast and it isn't on a network. That's the "closed circuit."

## The camera and the housing are separate

The big beige boxes you see on the corners of buildings usually aren't the camera itself. They're a metal housing with a sun shield on top. Inside is a small box camera about the size of a deck of cards, with a separate screw-on lens. Some housings also have a heater or a fan for outdoor use.

So a typical install is three parts you can buy separately:

1. The camera body (sensor and electronics)
2. The lens
3. The housing and mount

## Three kinds of "CCTV" camera

**Analog (composite video).** This is the old standard, used up to around 2010. The camera puts out a standard-definition video signal over coax with a BNC connector. You can plug it straight into a TV's yellow video input. The picture is 480i with a soft, classic security-footage look. This is what I'm working with.

**HD over coax (AHD, TVI, CVI).** These came later. They use the same coax cables but send HD video in one of three competing formats, and they only work with a DVR that supports that format. They won't show up on a normal TV. I avoided these.

**IP cameras.** These are network cameras. They use Ethernet, often get power over the same cable (PoE), and have a web page and an RTSP video stream. They're much higher resolution, but you're really learning networking, not the analog video side.

## Power

Analog cameras usually run on low voltage:

- **12 V DC**: from a plug-in adapter. With DC, + and - have to go to the right terminals.
- **24 V AC**: from a plug-in transformer, the same kind that powers doorbells and thermostats. With AC, the two wires can go either way.
- Many cameras accept both. Some older ones, like mine, are 24 V AC only.

The label on the camera says what it takes. "CLASS 2 ONLY / ISOLATED POWER ONLY" on the back just means to use a normal low-voltage plug-in supply, which is low power and safe to handle.

More on picking a supply in [power-and-wiring.md](power-and-wiring.md).

## The video signal

- Analog cameras output **composite video**: 1 volt peak-to-peak into 75 ohms, carried on coax.
- The connector on the camera is a **BNC**, a round metal plug with a twist-lock. TVs use **RCA** (the yellow jack), so a BNC-to-RCA cable or adapter connects the two.
- For long runs, installers use RG59 coax. "Siamese" RG59 has a power pair bundled with the coax so one cable carries both.

## NTSC vs. PAL

There are two analog TV standards:

- **NTSC**: North America and Japan, 525 lines, 60 Hz
- **PAL**: Europe and most other places, 625 lines, 50 Hz

A PAL camera won't display properly on a US TV. Model numbers usually give it away:

- JVC: **U** = US/NTSC, **E** = Europe/PAL (for example TK-C750U vs. TK-C750E)
- Samsung: **N** = NTSC, **P** = PAL
- A listing that says 230 V or 220 V is a European model

## Resolution in TV lines

Analog camera sharpness is measured in **TV lines (TVL)**, which counts how many vertical lines the camera can resolve across the picture. Late-90s color cameras are roughly 330-480 TVL. Later ones reach 600-700 TVL. Black-and-white cameras are usually sharper and better in low light than color ones from the same era.

## Lenses

- **C-mount vs. CS-mount**: the two standard threads. They have the same thread but sit at different distances from the sensor. A C lens fits a CS camera with a 5 mm adapter ring. A CS lens can't focus on a C camera.
- **Focal length**: smaller numbers mean wider. 2.8 mm covers a whole room, 12 mm is zoomed in.
- **Varifocal**: an adjustable zoom range, like 2.8-12 mm. You set it by hand, and then you have to refocus.
- **Iris**: a manual iris is set once. An auto-iris lens has a cable to the camera and opens and closes by itself as the light changes.
- **Back focus**: on box cameras, the lens mount itself can slide slightly to line focus up with the sensor. If a lens won't focus sharply across its whole zoom range, back focus is the adjustment to check. My camera has a BF LOCK screw for this.

## Line lock (LL) sync

Older camera systems often had many cameras feeding one monitor through a switcher. If each camera's video timing drifted on its own, the picture would roll every time the switcher changed cameras. **Line lock** fixes this by locking every camera's timing to the 60 Hz AC power line, so all cameras stay in step. That's one reason so many older cameras run on 24 V AC. The PHASE adjustment fine-tunes the lock.

With a single camera, internal sync (INT) is fine.

## Night vision

Many cameras switch to black and white in the dark and use infrared light (IR LEDs) that the sensor can see but people can't. Cameras without built-in IR, like mine, show a black picture in a dark room unless you add a separate IR illuminator.
