---
title: Lora Puck
author: Liz
description: A Lora module with a AHT20 sensors and LCD display to show status
created_at: 2026-07-16
---
### Total time spent: 9 Hours

## Day 1 - Getting started! - July 16th - 2.5 Hours
I wanted to make a Lora Puck to learn more about frequency and radio wave.
I read through the [Lora guide](https://stasis.hackclub.com/starter-projects/meshtastic-lora) to learn about the basics, the schematic connection and pcb layout. 

Starting with the schematic, I connect the decoupling capacitors, resistors, antenna chip according to the guide. 
I added battery management system as well because I want it to be portable and I need to charge the battery. I went online to look for a suitable battery management system and the datasheet. Referring to the example application circuit, I drew a function block for that.  Then, I went to double check those connection. 
<img width="427" height="458" alt="Screenshot 2026-08-21 at 3 04 36 PM" src="https://github.com/user-attachments/assets/f7779aba-4f75-4208-9443-e8b12e678b5f" />

### PCB Layout Time!!
I carefully take note of which capacitor need to be close with which pins to lower the noise. I group the components together with their function block. Then I only start placing them as compact as possible as I want the board to be small. 

Then I started routing. I tried to routed the antenna as short as possible. Then the differential pair (USB +-) and power lines. And finally the other lines. 

## Day 2 - Routing + Fix DRC errors - July 17th - 1.2 Hours

I finished routing the board. 
Initially, I planned to pour ground plane on the bottom copper layer and 3v3 plane on the top copper layer. But considering it might affect the impedance of the board and change the antenna magnetic field, I choose a safer path, which is to pour ground on both copper layer. 

Then i when through all the errors, mostly are just some connection i missed out to connect, but I was stuck at one of the error which told me to connect from copper plane to copper plane. I couldn't find what's wrong with it. 
With advice from slack, I put some sticthing vias to fix the problem.

<img width="519" height="605" alt="Screenshot 2026-08-21 at 3 02 46 PM" src="https://github.com/user-attachments/assets/a1ddf047-756a-4528-b425-d76db07a716e" />

## Day 3 - Modifying Design - July 22th - 2 Hours

I took a break from this project to work on my other project. 
After coming back, I decided to add a humidity sensor and a e-ink display to my Lora module so it can send data via the Lora and display.

<img width="264" height="142" alt="Screenshot 2026-08-21 at 3 26 47 PM" src="https://github.com/user-attachments/assets/b1cfa6a5-e65a-4611-a3fe-db70b21f5338" />

Transforming a simple Lora module into a weather monitor device. Increasing it's functionality.

I went to check the pins to make sure they are compatible.

<img width="899" height="600" alt="Screenshot 2026-08-13 at 10 35 21 PM" src="https://github.com/user-attachments/assets/200c9cb5-e874-4d79-8524-df71a9b7d31b" />

Since I can’t find footprint for the display and sensors, I drew it myself.

## Day 4 - Rerouting - July 23th - 1.5 Hours

Since I added some new components, I have to modify the placement of the components and reroute it.

<img width="424" height="245" alt="Screenshot 2026-08-21 at 4 37 43 PM" src="https://github.com/user-attachments/assets/fb993bfe-5454-421c-bc88-554454aad9c0" />

## Day 5 - Change Display - August 12th - 0.5 hours

After reviewing the new version of the pcb, the e-ink display that I picked earlier made the device too big and awkward to carry around. So I changed the e-ink display to a smaller 0.96 inch LCD display. Now it looks much more compact and better to carry around.

<img width="548" height="459" alt="Screenshot 2026-08-21 at 4 52 24 PM" src="https://github.com/user-attachments/assets/33cbb14d-45e7-4f38-9959-e0fe5f1a06b9" />

## Day 6 - Rerouting & Double check  - August 12th - 1.2 hours

I rerouted some lines. I was trying to make the lines from the antenna chip to the esp chip more neater with enough spacing to prevent interference of magnetic field. It took me some experiments before finding the best way to route it. Finally I went on to double check everything and added text on the PCB.



