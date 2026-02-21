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

<img width="1420" height="632" alt="Render-1" src="https://github.com/user-attachments/assets/ae9167f8-3e1a-413b-99a2-643bd582d354" />








## BOM

# Bill of Materials (BOM)

Conversion rate used:  
**1 USD = ₹91.63**

| Item | Part Name | Qty | Unit Price (INR) | Unit Price (USD) | Link |
|------|-----------|-----|-----------------|-----------------|------|
| 1 | Raspberry Pi Pico H | 1 | 469 | 5.12 | https://robocraze.com/products/raspberry-pi-pico-h-pico-with-headers-soldered?variant=43243705467104 |
| 2 | MG995 Servo Motor | 1 | 226 | 2.47 | https://robocraze.com/products/mg995-servo-motor?variant=40193009844377 |
| 3 | HC-SR04 Ultrasonic Sensor | 1 | 71 | 0.77 | https://robocraze.com/products/hc-sr-04-ultrasonic-sensor?_pos=1&_psq=ultrasonic&_ss=e&_v=1.0 |
| 4 | Potentiometer | 1 | 95 | 1.04 | https://robocraze.com/products/potentiometer-knobs-pack-of-10?_pos=5&_sid=d19dd35bb&_ss=r |
| 5 | SSD1306 OLED Display | 1 | 161 | 1.76 | https://robocraze.com/products/0-96in-oled-display-module-4pin?variant=40192586645657 |
| 6 | Push Buttons | 1 | 16 | 0.17 | https://robocraze.com/products/4-pins-dip-momentary-square-tactile-push-button-switch-10-pieces-6x6x5mm?variant=43223713874144 |
| 7 | Passive Buzzer Module | 1 | 27 | 0.29 | https://robocraze.com/products/passive-buzzer-module?_pos=3&_sid=93d5392af&_ss=r |
| 8 | 10k Ohm Resistor Pack | 1 | 11 | 0.12 | https://robocraze.com/products/10k-resistor-pack-of-10?_pos=1&_sid=70ca973f2&_ss=r |
| 9 | Breadboard | 1 | 71 | 0.77 | https://robocraze.com/products/breadboard?_pos=3&_sid=273252606&_ss=r |
|10 | Jumper Wires Set | 1 | 128 | 1.40 | https://robocraze.com/products/jumper-wire-set-m2m-m2f-f2f-40-pcs-each?_pos=2&_sid=bf44cc87d&_ss=r |

## Checkout page:
<img width="1855" height="870" alt="{C71266C3-8C01-4ECC-98E7-B6AF25E16808}" src="https://github.com/user-attachments/assets/4537303b-e9df-4d49-b2e4-cba1340138ca" />


Note: I have not inlcuded bread board in the cad because it was not part of the final product.
But I really need one.

Thanks!


## Total
| Currency | Total |
|----------|--------|
| INR | **₹1275** |
| USD | **$13.92** |



Note - I edited the BOM with new links/suppliers and I replaced esp32 s3 c1 n8r8 with RaspberryPi pico since I didnt need wifi or bluetooth module.
