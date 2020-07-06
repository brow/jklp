# jklp

**jklp** (pronounced like "jökulhlaup") is an ergonomic keyboard with just 36 keys. It's designed around the natural resting position of your hands.

Compared to other minimal ergonomic keyboards, its unusual features are:
* High angle between halves (20°) that can be altered without rewiring
* Extreme pinky stagger

This repository contains the files you need to make a functioning jklp from scratch, including the case, wiring, and firmware.

The design requires ALPS-style switches and a Pololu A-Star controller. You won't need a PCB or hot glue.

![photo of jklp keyboard](https://user-images.githubusercontent.com/238331/86539100-b0a73300-bebf-11ea-84c8-a45621be50af.png)

_jklp including parts from an Apple Extended Keyboard II_.

## Case

![diagram of case](https://user-images.githubusercontent.com/238331/74681252-83fcb400-5188-11ea-9273-33d56c56d01d.png)

The case is a stack of laser-cut layers fastened together by bolts. The layers are:

### Base

![diagram of base](https://user-images.githubusercontent.com/238331/74681918-35501980-518a-11ea-973c-642ae579af5a.png)

The base is single piece that holds the halves of the keyboard together and sets their angle with respect to one another. It can be of any thickness or material. I used 1/4" plywood.

The base included in `case.svg` sets an angle of 20°, but you can make another base with a different angle and swap it in anytime, even after wiring.

### Frame

![diagram of base](https://user-images.githubusercontent.com/238331/74682049-94159300-518a-11ea-898a-348a0ce69fe8.png)

The frame creates a cavity for the wiring, contacts, and diodes. It can be of any material but should be at least 5 mm thick.

### Plates

![diagram of plates](https://user-images.githubusercontent.com/238331/74682100-ba3b3300-518a-11ea-9568-aab6cd259947.png)

The plates hold the switches firmly in place, avoiding the need for a PCB or hot glue. The plates have two layers:
* A 1/16" acrylic layer that ALPS-style switches "click" snugly into.
* Another, thicker layer to add rigidity.

### Crystal

![diagram of crystal](https://user-images.githubusercontent.com/238331/74682170-ed7dc200-518a-11ea-9cc5-e79c02d5a6ec.png)

The crystal is an optional shield over the controller (not pictured in the photo at top). Like the [base](#base), this piece needs to be replaced in order to change the split angle, and the included one is for a 20° angle.

## Wiring and firmware

![wiring diagram](https://user-images.githubusercontent.com/238331/86537993-b8afa480-beb8-11ea-801e-b35586f2f2f0.png)

The wiring of the key matrix and controller is specified by `firmware.json`, which can be edited and compiled to corresponding firmware in [Keyboard Firmware Builder].

If you don't understand what that means or need help with wiring technique, the [QMK Hand Wiring Guide] is good.

### Layout file

To play with the layout or redesign the key matrix from scratch, start by opening up `layout.json` in the [Keyboard Layout Editor].

![animated blinking controller](https://user-images.githubusercontent.com/238331/86539735-9cb20000-bec4-11ea-9028-98b84af8b08a.GIF)

[Keyboard Firmware Builder]: https://kbfirmware.com
[Keyboard Layout Editor]: http://www.keyboard-layout-editor.com
[QMK Hand Wiring Guide]: https://beta.docs.qmk.fm/using-qmk/guides/keyboard-building/hand_wire
