# Stardeck

A minimalist cyberdeck made for a software guy to learn embedded systems, electronics, and hardware design.
Made for Hack Club's 2026 Stardance Challenge.

Learn more here: https://stardance.hackclub.com/

View my project on Stardance here: https://stardance.hackclub.com/projects/19479

## Overview

This cyberdeck is made for teaching me the art of hardware through doing. I've been interested in cyberdecks ever since first seeing them in a post on r/cyberdeck, and I'm looking forward to manifesting that interest by making my own. Instead of buying a built device online, I wanted to learn how designing hardware works - from ideas to plans to products. Having the ability to add even a few lines of code to a repo you may be working on using a device that doesn't take up that much space is just one possibility with cyberdecks, with many others opening up once I get a working prototype built.

## Design Philosophy

Stardeck is designed and built using inexpensive components and open-source tools that ensure that anyone could build their own Stardeck.

The first revision will target simplicity and learning through engineering design, which will enable me in future revisions to improve upon Stardeck by testing it in the real world.

## Goal

**First Goal:** Build the ugliest functional cyberdeck possible this summer and submit it to Stardance.

Stardeck prioritizes functionality and learning over aesthetics for its first version. Once the system is operational, later iterations will focus on usability, appearance, and additional features. This approach prioritizes reaching a working MVP before focusing on aesthetics or refinement (although, those can be reached once we actually have something that boots).

## Hardware

The hardware required for this first version is very minimal, with every part having a purpose that directly translates to functionality. Technical details can be reduced by breaking down my project into its main components:

Computer: The brain behind Stardeck doesn't need much space, but it has much to offer - The Raspberry Pi. This single-board computer has the ability to run an OS, surf the web, connect external devices, and more, while also able to fit into my pocket.

Display: Many of these don't take up too much space but still can connect to a Pi for easy output.

Power Bank: This portable recharge base is what gives this valuable resource to all the other components.

Storage: The Pi needs an OS to run on, and that OS needs storage for the Pi to boot from. A microSD card should have enough storage to comfortably boot an OS and store any necessary files once booted.

Video Adapter: In the case where the display uses HDMI input which doesn't fit with the Pi's micro-HDMI output, an adapter will allow both components to connect to each other regardless.

Keyboard: An external USB keyboard, which I will provide, will be required to make sure the MVP can take inputs.

Flash Drive: If any more storage is owned, the Pi can access files from a Flash Drive I already own that should have enough storage for Stardeck to live off of.

## Bill of Materials (BOM)

| Component | Model | Qty | Cost | Link |
|-----------|--------|----:|-----:|------|
| Computer | Raspberry Pi 4 Model B (4GB RAM) | 1 | $79.95 | [Canakit](https://www.canakit.com/raspberry-pi-4-4gb.html?cid=USD) |
| Display | Elecrow RC070 7-inch Touchscreen Display (1024×600) | 1 | $54.99 | [CrowPi](https://www.crowpi.cc/products/rc070-7-inch-raspberry-pi-monitor-1024x600-touchscreen-mini-hdmi-lcd-screen?variant=39701750775941&country=US&currency=USD&utm_source=chatgpt.com&oppcref=e96bec25-1e39-4ef8-afa0-9b23e74db94f) |
| Power Bank | Anker 10000mAh Portable Charger | 1 | $19.99 | [Amazon](https://www.amazon.com/Anker-Travel-Ready-Technology-High-Speed-Output%EF%BC%88Black%EF%BC%89%EF%BC%8C1pack/dp/B0D5CLSMFB?th=1) |
| Storage | SanDisk Ultra Plus 64GB microSDXC UHS-I Memory Card | 1 | $14.00 | [Best Buy](https://www.bestbuy.com/product/sandisk-ultra-plus-64gb-microsdxc-uhs-i-memory-card/JXJ62C647Q) |
| Video Adapter | Micro HDMI to HDMI Adapter Cable (6 inch) | 1 | $3.64 | [Walmart](https://www.walmart.com/ip/Micro-HDMI-to-HDMI-Adapter-Cable-4K-60Hz-15cm-6-inch-Short-Cord-for-Raspberry-Pi-5-4-Camera-Tablet-HDTV/19994810413?wmlspartner=wlpa&selectedSellerId=103086963&veh=seo_fpl&cn=google) |
| Keyboard | Existing USB Keyboard | 1 | $0.00 | Already owned |
| Flash Drive | Existing 128GB USB Flash Drive | 1 | $0.00 | Already owned |

**Estimated Total Project Cost:** $172.57

## System Architecture

Stardeck can be broken down into four subsystems - power, computing, input, and output - that interact as outlined below. The biggest challenge that came from planning out component interactions is that I did not have the actual parts at hand at that time, so I had to gain experience with designing around parts that only existed in ideation. Putting them into designs ended up answering the question of how Stardeck works electrically.

![System Architecture](assets/schematics/System-Architecture-A2.png)
![Engineering Notes](assets/schematics/Engineering-Notes.png)

## Progress

- [x] Selected hardware
- [x] Created wiring diagram
- [x] Created BOM
- [x] Designed enclosure
- [x] Completed packaging study
- [ ] Print first prototype
- [ ] Assemble hardware
- [ ] Install Raspberry Pi OS
- [ ] Boot v0.1

## Roadmap

### Near-term
- Print enclosure
- Assemble electronics
- Boot Raspberry Pi OS
- Validate packaging

### Long-term
- Integrated 60% keyboard
- SSD
- Modular expansion
- Improved enclosure

These enhancements are intentionally deferred until the initial prototype validates Stardeck's core terminal and file-management workflows.

## Current Status
Planning

## Learn More
Visit the `docs` folder to follow the project's development through design notes and devlogs.