# Initial Schematic

_Note: This is simply a system schematic to understand how components in the cyberdeck will interact with one another, apired with a packaging study to understand how much space each part takes up in our chosen arrangement. Nothing too crazy for now._

With ideation for designs in place, it's easy to jump into the technical details first. However, that's for sometime later. This document focuses on the abstracted interactions between the power, the Raspberry Pi (I chose to go with a Raspberry Pi 4B), the screen, and the keyboard. After we figure out these interactions, we can take note of dimensions and (hopefully?) get a physical representation of our current parts onto Onshape so we can design a starting case. The starting question was:

What parts will Stardeck consist of, and how do they interact with one another?

Here's what I managed to identify about the major subsystems and their relationships through investigation.

## Questions Answered
The cyberdeck consists of four primary subsystems:
- Power
- Computer
- Input
- Output

## System Schematic (acting as our initial plan)
![System Schematic](../assets/schematics/System-Schematic.png)

## Descriptions:
- The power subsystem provides energy to all the other subsystems. This is the cornerstone of Stardeck.
- The computer acts as the central controller. It manages the actions of input and output.
- The keyboard serves as the primary input device. Makes sense - typing will be the main source of input as other input sources (coming through extra USB ports for other devices) can be figured out later, especially if the display is touch-screen.
- The display serves as the primary output device. It shows you what's going on.

## Open Questions
- Which display to buy?
- How large should the battery be?
- Integrated keyboard or external keyboard?
- Approximate enclosure dimensions?

I was able to follow along with this intuitively. After this, I looked into many cyberdeck designs available publicly (r/cyberdeck was _) and decided on a compact, tablet-like cyberdeck.

This will consist of a screen inserted into the front face and the Pi and power bank put onto the back face, using up the room left by the shelled case. This is the most efficient design to aim for as of right now since we're only aiming to boot it up for this version. In future versions, we can make the screen rotate to face you laptop-style for a better feel.

## Packaging Study Findings

These were the initial, "best guess" dimensions inside the placeholder based on guesswork:

(All 3D dimensions listed are in the form length x width x height.)

- **Case**: 230 mm x 160 mm x 40 mm, 
_(with a cut-out openong on the top face to make room for the inserted screen.)_

- **Screen**: 200 mm x 120 mm x 15 mm

- **Raspberry Pi 4B**: 90 mm x 60 mm x 25 mm

- **Power Bank**: 110 mm x 70 mm x 20 mm

The initial screen placeholder was too big to match the intended size.

The original placeholder measured approximately 200 mm × 120 mm, resulting in a diagonal of ~33 mm (~9.2 inches). However, the intended display size is 7 inches. The placeholder was revised to:

- **Screen (7")**: 155 mm x 87 mm x 15 mm,

yielding a diagonal measurement consistent with a 7-inch display.

This change made me more conscious about lowering the enclosure footprint in other ways, too, so I looked into the accuracy of the rest of the designs.

The case size would be able to fit everything in practice, since its placeholder assembly in Onshape was able to fit everything neatly inside of it (or inserted onto it, in the screen's case). The Raspberry Pi's placeholder was close enough in size to the actual thing, but with some more cubic millimeters added in to account for wires, tolerances, and whatever else the actual build would throw at us. As for the battery pack, though, I haven't selected anything specific just yet. Because of this, the battery pack's placeholder are based on estimates and should be updated once a specific battery model is selected. Speaking of selection, note that the battery dimensions are preliminary estimates based on a typical 10,000 mAh USB power bank and should be updated after choosing our final power source (something rechargeable from Anker, perhaps).

With these in mind, here was the placeholder assembly used for the packaging study:

![Placeholder Assembly (Top)](../assets/cad/Placeholder-Assembly-Top.png)

![Placeholder Assembly (Bottom)](../assets/cad/Placeholder-Assembly-Bottom.png)

So far, the parts we will be using seem to interact with each other clearly and fit into one coherent assembly. For next steps, we'll figure out how we can get the parts in question to work together and turn into a real plan/schematic.

God bless you,
^ Yodahe