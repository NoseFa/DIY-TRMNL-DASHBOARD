# Nordic TRMNL

A diy dashboard that is built with the TRMNL software in mind. Can display stuff like the your calendar, reminders or the public transit schedule. This repo is only for the hardware side. The TRMNL docs were a huge help in the design process and most of the electronics are based on their suggestions. This project was designed as a part of the HackClub hardware hackathon FALLOUT where people make hardware projects and get a chance to go to Shenzhen, China. More info available here [Fallout](https://fallout.hackclub.com)!

## Parts

- SEEED studio 7.5" monochrome e-ink display
- SEEED studio ePaper driver board
- SEEED studio XIAO ESP32-C3
- 3D printed [Case](./3Dfiles/)

## Software

I will be using the opensource TRMNL software and will be self-hosting the server. If you are replicating my design but can't self-host there is a one time purchase of 43,95€ to use TRMNL servers. TRMNL software Github [Repo](https://github.com/usetrmnl/trmnl-firmware) and TRMNL website [Trmnl.com](https://trmnl.com/). TRMNl has a large [plugin environment](https://trmnl.com/integrations) and a user made [Recipes](https://trmnl.com/recipes). These plugins are the life blood of the device in my opinion and makes it possible to customize what is displayed according to what you need. For example if you are interested Formula 1 you can use the Formula 1 plugin to follow the races.

## Build guide

If you are using the same components you can print the case available here [3D files](./3Dfiles). [Case only folder](./3Dfiles/CaseOnly) has ready to print files that only have the case. Use these if you are just printing the case. The [full project folder](./3Dfiles/FullProject) has the whole Fusion project including the driver board PCB and the display. You might want to use this if you want to edit the files.

Attach the ESP32 to the driver board using the pins and then connect the display to the driver board. The display should be installed in the case first and the cable routed through the hole made for it. The driver board has holes for you to press in heated inserts and then you can screw in 2.5mm screws in to attach the board to the case. Finally flash the software and plug in usb-c power. Then just walkthrough the device setup based on if you are using TRMNL servers or self-hosting.

If self-hosting follow the up to date guide available in the TRMNL dev [docs](https://docs.trmnl.com/go/diy/byod-s). This is the guide I used for my setup.

If you plan on using TRMNL servers. After flashing the firmware you have to buy access and then claim the device through the site. [Claim your device](https://trmnl.com/claim-a-device). Then you can follow the instructions given on the TRMNL dev [docs](https://docs.trmnl.com/go/diy/byod).

For mounting I used command strips / double sided tape. I think this is better than screws for example because the device is light enough to just be held up with double sided tape. Also making the device attach with screws reliably would be harder and in my opinion overkill.

## Why does this exist ?

This was a personal project made to make my day to day life easier. Every morning when I wake up I first open my school schedule then check the time and finally the public transit schedule. Of course because of early mornings I usually had to check atleast twice. So I looked for solutions of displaying a calendar. I needed it to be digital because I didn't have energy to use a paper calendar. So I found the TRMNL which was a perfect solution for my problem. Unfortunately the official TRMNL OG was a bit too expensive and didn't come with a wall mount. So I decided to make my own.

### Why it's a bit better ?

So the my diy Nordic TRMNL is made to be wall mountable. This makes it easier to blend in to the environment. Also buying the components directly and self hosting the server makes the whole package a little bit cheaper. I still am thankful that TRMNL decided to open source the software and make the product diyable and self hostable. So there are somethings that I think my TRMNL is better for.

## Zine Page

![Zine Page](./Media/TrmnlZinePageScreenshot.png "Zine Page")

## Excalidraw / Notes

I used excalidraw during my design process. The mind map screenshot attached has most of my design notes.
![Excalidraw](./Media/TrmnlExcalidraw.png "Excalidraw")

Bill of Materials available here: [BOM](./BOM.csv)

## Pictures

Here are some more pictures of the project.

![Case with PCB](./Media/CaseWithScreen.png "Case with PCB")
Case from behind with screen and PCB.

![Case](./Media/OnlyCase.png "Case without PCB")
Case from the front without screen and PCB.
