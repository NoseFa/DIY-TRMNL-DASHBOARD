# Nordic TRMNL

A diy dashboard that is built with the TRMNL software in mind. Can display stuff like the your calendar, reminders or the public transit schedule. This repo is only for the hardware side. The TRMNL docs were a huge help in the design process and most of the electronics are based on their suggestions. This project was designed as a part of the HackClub hardware hackathon FALLOUT where people make hardware projects and get a chance to go to Shenzhen, China. More info available here [Fallout](https://fallout.hackclub.com)!

## Parts

- SEEED studio 7.5" monochrome e-ink display
- SEEED studio ePaper driver board
- SEEED studio XIAO ESP32-C3
- 3D printed [Case](./3Dfiles/)

## Software

I will be using the opensource TRMNL software and will be self-hosting the server. If you are replicating my design but can't self-host there is a one time purchase of 43,95€ to use TRMNL servers. TRMNL software Github [Repo](https://github.com/usetrmnl/trmnl-firmware) and TRMNL website [Trmnl.com](https://trmnl.com/).

## Build guide

If you are using the same components you can print the case available here [3D files](./3Dfiles/). Attach the ESP32 to the driver board using the pins and then connect the display to the driver board. The display should be installed in the case first and the cable routed through the hole made for it. The driver board has points on the case that can attach to the case. Finally flash the software and plug in usb-c power. Then just walkthrough the device setup based on if you are using TRMNL servers or self-hosting.

If self-hosting follow the up to date guide available in the TRMNL dev [docs](https://docs.trmnl.com/go/diy/byod-s). This is the guide I used for my setup.

If you plan on using TRMNL servers. After flashing the firmware you have to buy access and then claim the device through the site. [Claim your device](https://trmnl.com/claim-a-device). Then you can follow the instructions given on the TRMNL dev [docs](https://docs.trmnl.com/go/diy/byod).

## Zine Page

![Zine Page](./Media/TrmnlZinePageScreenshot.png "Zine Page")

## Excalidraw / Notes

I used excalidraw during my design process. The mind map screenshot attached has most of my design notes.
![Excalidraw](./Media/TrmnlExcalidraw.png "Excalidraw")

Bill of Materials available here: [BOM](./BOM.csv)

