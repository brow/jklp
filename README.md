# jklp

![photo of jklp](https://user-images.githubusercontent.com/238331/74573434-43155d00-4f46-11ea-8c16-44160e10b993.JPG)

**jklp** (pronounced like "jökulhlaup") is a computer keyboard that is 40%, unsplit, and very column-staggered.

Its most unusual features are:
* High angle between halves (20°) that can be changed without rewiring
* Extreme pinky stagger
* Glue-less, PCB-less construction

This repository contains the files you need to make a functioning jklp from scratch, including the case, hand-wiring, and firmware.

The design requires ALPS-style switches and a Pololu A-Star controller.

## Case

![diagram of case](https://user-images.githubusercontent.com/238331/74681252-83fcb400-5188-11ea-9273-33d56c56d01d.png)

The case is a stack of laser-cut layers fastened together by bolts.

### Base

![diagram of base](https://user-images.githubusercontent.com/238331/74681918-35501980-518a-11ea-973c-642ae579af5a.png)

The base is single piece that holds the halves of the keyboard together and fixes their angle with respect to one another. It can be of any thickness or material. I used 1/4" plywood.

The base included in `case.svg` fixes an angle of 20°, but you can make your own base with a different angle and swap it in anytime, even after wiring.

### Frame

![diagram of base](https://user-images.githubusercontent.com/238331/74682049-94159300-518a-11ea-898a-348a0ce69fe8.png)

The frame creates a cavity for the wiring, contacts, and diodes. It can be of any material but should be at least 5 mm thick.

### Plates

![diagram of plates](https://user-images.githubusercontent.com/238331/74682100-ba3b3300-518a-11ea-9568-aab6cd259947.png)

The plates hold the switches firmly in place, eliminating the need for a PCB or hot glue. They are each made of two layers:
* A 1/16" acrylic layer that ALPS-style switches "click" snugly into.
* Another, thicker layer to add rigidity.

### Crystal

![diagram of crystal](https://user-images.githubusercontent.com/238331/74682170-ed7dc200-518a-11ea-9cc5-e79c02d5a6ec.png)

The crystal is an optional shield over the controller (not shown in the photo at top). Like the base, this piece needs to be replaced in order to change the split angle, and the included one is for a 20° angle.

## Wiring

TODO

## Firmware

TODO

## Glossary

* "40%" means it has about 40% as many keys as full-sized board. Typing a given character sometimes requires pressing a combination of keys.
* "Unsplit" means it resembles a split keyboard in that has a distinct half for each hand, and the halves are angled inward to match the angle of your resting forearms. But it's unsplit because the two halves are joined together.
