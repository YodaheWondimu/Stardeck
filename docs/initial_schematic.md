# Initial Schematic

_Note: This is simply a system schematic to understand how components in the cyberdeck will interact with one another. Nothing too crazy for now._

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