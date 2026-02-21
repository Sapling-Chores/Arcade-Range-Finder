<img width="1420" height="632" alt="Render-1" src="https://github.com/user-attachments/assets/2112e000-d348-405f-afad-ec5b9a830d1e" />


# Arcade-Range-Finder

## What this project do?
Arcade-Range-Finder is a raspberry pi pico based range finder which uses Ultrasonic sensor and oled display to show the range in a very unique way.
This project has three modes controlled by pushButtons. 
Mode 1 & 2: Radar like display which shows Blits when an object is detected in range.
Mode 1 Specific - Manual Cntrol servo with Potentiometer.
Mode 2 Specific - Servo runs in loop.

Mode 3: Servo runs on loop.  But in oled everytime the range changes, new ball is displayed and most prior ball gets removed from the screen. And every ball's speed is determined by the mapped distance to the speed of ball.
We also have small box which copies the x-cordinates of ball so everytime ball touches the box the ball gets bounced back.

## Why I made this ?

I have seen multiple range finder but almost all of them had radar like display, but I wanted to do something different and unique.


# Schematics:
<img width="1202" height="715" alt="{34E696DF-806E-4F16-AFEF-69D0F57188B0}" src="https://github.com/user-attachments/assets/8c961f5b-97aa-4ffa-b78f-c5ad960e567a" />
<img width="1639" height="768" alt="{3B086E0B-E55D-48C3-B064-536685C85CE2}" src="https://github.com/user-attachments/assets/2cf545f6-51ee-4cf0-9c01-930daa81d2fe" />

Cad:

<img width="1219" height="729" alt="{B3FAAC0A-0B31-4C0B-A097-FDF3A977DD9B}" src="https://github.com/user-attachments/assets/16b011bd-acd2-4439-8f7d-0586f62fa6af" />

<img width="1305" height="811" alt="{6561AC41-3016-4171-98F6-8D0EDA1C9C4F}" src="https://github.com/user-attachments/assets/63234076-bb54-4371-8d8c-1476ae833c4b" />


<img width="1420" height="632" alt="Render-1" src="https://github.com/user-attachments/assets/ae9167f8-3e1a-413b-99a2-643bd582d354" />








## BOM

# Bill of Materials (BOM)


| S No | Item | Unit/Pieces | Price (Rs) | Price ($) | Link |
|---|----|---------|---------|-------|------|
| 1 | Raspberry Pi Pico 2 W | 1 | 738 | 8.13 | https://robu.in/product/raspberry-pi-pico-2-w/ |
| 2 | MG995 Servo | 1 | 240 | 2.65 | https://robu.in/product/towerpro-mg995-metal-gear-servo-motor/ |
| 3 | HC-SR04 Ultrasonic Sensor | 1 | 74 | 0.82 | https://robocraze.com/products/hc-sr-04-ultrasonic-sensor |
| 4 | SSD1306 0.96 OLED 128x64 | 1 | 219 | 2.41 | https://robu.in/product/0-96-oled-display-module/ |
| 5 | 4-Pin Tactile| 10 pcs | 16 | 0.18 | https://robocraze.com/products/4-pins-dip-momentary-square-tactile-push-button-switch-10-pieces-6x6x5mm |
| 6 | Buzzer Module | 1 | 24 | 0.26 | https://robu.in/product/smartelex-passive-buzzer-module/ |
| 7 | 10k Ohm 0.25W Resistor | 100 pcs | 29 | 0.32 | https://robu.in/product/10k-ohm-0-25w-metal-film-resistor-pack-of-100/ |
| 8 | Breadboard | 1 | 61 | 0.67 | https://robu.in/product/mb102-830-points-solderless-prototype-pcb-breadboard-high-quality/ |
| 9 | Jumper Wire Set | 1 | 128 | 1.41 | https://robocraze.com/products/jumper-wire-set-m2m-m2f-f2f-40-pcs-each?variant=40192573636761 |
| 10 | 10k Rotary Potentiometer| 5 pcs | 66 | 0.73 | https://robocraze.com/products/10k-ohm-16mm-rotatory-variable-potentiometer-pack-of-5 |
| 11 | Shipping (Robocraze) | 1 | 49 | 0.54 | - |
| 12 | Shipping (Robu.in) | 1 | 0 | 0.00 | - |
|  | **Total** |  | **1644** | **18.12** | - |



Note : I updated checkout pages because there were some components out of stocks.
## Checkout page:
<img width="1578" height="758" alt="{BFEC8E5B-52E8-446E-9A52-B848A6E4B4C5}" src="https://github.com/user-attachments/assets/8f98bfcf-c2e6-462c-a467-0d8d6df399ee" />

<img width="1125" height="746" alt="{752DBDBF-14D5-43F9-848D-CDFD90AA3417}" src="https://github.com/user-attachments/assets/759007c8-d27f-4e85-b733-8ad2eb8b604f" />




Note: I have not inlcuded breadboard in the cad because it was not part of the final product.
But I really need one.

Thanks to :

my mum , my dad, hackclub and blueprint.
and blueprint staffs who works really well!



