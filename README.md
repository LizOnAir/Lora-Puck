# Lora-Puck
A Lora module with a AHT20 sensors and LCD display to show status. I made this to discover about how to use LoRa for communication.

<img width="350" height="290" alt="Screenshot 2026-08-31 at 10 58 07 PM" src="https://github.com/user-attachments/assets/fa24f3ef-2c51-4ce0-ad27-39ff24ed19dd" />

## Features:
- detect humidity
- detect temperature
- send data via Lora
- low power consumption
- display

## PCB
<img width="672" height="524" alt="PCBMODEL" src="https://github.com/user-attachments/assets/2b0358c4-e8d6-4322-8a1e-a95c31f9b4c6" />

### Schematic
<img width="899" height="600" alt="Screenshot 2026-08-13 at 10 35 21 PM" src="https://github.com/user-attachments/assets/7c2c00da-1fc9-49ab-9124-7721c84a91b7" />

### Layout
<img width="464" height="396" alt="Screenshot 2026-08-13 at 10 35 02 PM" src="https://github.com/user-attachments/assets/6c604c48-d9b8-4b38-b545-001f77935a08" />
<img width="464" height="396" alt="Screenshot 2026-08-13 at 10 35 05 PM" src="https://github.com/user-attachments/assets/d70c93c2-cb01-4fff-b42e-3beb82e868a0" />

Access files in [PCB folder](https://github.com/LizOnAir/Lora-Puck/tree/main/PCB).

For this design, I'm using PCBA from JLCPCB.

## CAD
<img width="350" height="290" alt="Screenshot 2026-08-31 at 10 58 07 PM" src="https://github.com/user-attachments/assets/6d933feb-2df1-4922-b3d1-70085fe16d67" />
<img width="350" height="290" alt="Screenshot 2026-08-31 at 10 58 02 PM" src="https://github.com/user-attachments/assets/4a2a1cd8-1173-4cf7-8463-c6cd29f3bcee" />
<img width="350" height="290" alt="Screenshot 2026-08-31 at 10 58 21 PM" src="https://github.com/user-attachments/assets/c3002d3f-2b18-482f-bdd6-5e2e9b83e267" />

Made in Fusion360.Liz
Access files in [CAD folder](https://github.com/LizOnAir/Lora-Puck/tree/main/CAD).

### Assembly
1.  Insert 4 heatset onto the 4 mounting holes in the bottom case.
2.  Insert the PCB into the bottom case.
3.  Using hot glue, stick the buttons onto the tactile switches.
4.  Align the holes of PCB onto the holes of the bottom case.
5.  Cover the top case over the bottom case.
6.  Screw them tight together.
7.  Charge the battery and hang it on somewhere to start detect temperature!!

## Firmware
I use Arduino IDE for programming.
- display
- sensors
- sending data via lora

Access files in [Firmware folder](https://github.com/LizOnAir/Lora-Puck/tree/main/Firmware).
