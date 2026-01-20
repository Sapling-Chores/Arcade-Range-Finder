# Arcade-Range-Finder

## What this project do?
Arcade-Range-Finder is a Esp32 based range finder which uses Ultrasonic sensor and oled display to show the range in a very unique way.
This project has three modes controlled by pushButtons. 
Mode 1 & 2: Radar like display which shows Blits when an object is detected in range.
Mode 1 Specific - Manual Cntrol servo with Potentiometer.
Mode 2 Specific - Servo runs in loop.

Mode 3: Servo runs on loop.  But in oled everytime the range changes, new ball is displayed and most prior ball gets removed from the screen. And every ball's speed is determined by the mapped distance to the speed of ball.
We also have small box which copies the x-cordinates of ball so everytime ball touches the box the ball gets bounced back.

## Why I made this ?

I have seen multiple range finder but almost all of them had radar like display, but I wanted to do something different and unique.


# Schematics:
<img width="1000" height="1076" alt="Schematics" src="https://github.com/user-attachments/assets/148f428e-7514-49a3-9115-b7ddd1f788f8" />

## BOM

| Item no. | Component           | Specs/Model                  | Price (INR) | Price (US$) | Item link |
|----------|-------------------|------------------------------|-------------|-------------|-----------|
| 1        | ESP32 devkit       | ESP32‑S3‑DevKitC‑1‑N8R8      | ₹1,194.87   | $13.14      | [Link](https://www.mouser.in/ProductDetail/Espressif-Systems/ESP32-S3-DevKitC-1-N8R8?qs=7D1LtPJG0i2PiuUUKucutQ%3D%3D&mgh=1&utm_source=chatgpt.com) |
| 2        | OLED display       | SSD1306 OLED 128x64           | ₹520        | $5.72       | [Link](https://www.amazon.in/Robocraze-Inches-Display-Module-Arduino/dp/B077TH5WWY) |
| 3        | Ultrasonic Module  | HC‑SR04 Ultrasonic            | ₹190        | $2.09       | [Link](https://www.amazon.in/Banggood-Ultrasonic-Distance-Measuring-Transducer/dp/B01I1ZTPJC) |
| 4        | Potentiometer      | 10k 3‑Pin                     | ₹111        | $1.22       | [Link](https://www.amazon.in/Electronic-Spices-Potentiometer-Multiple-Applications/dp/B0CP9NNMH3) |
| 5        | Servo Motor        | SG90 Micro                     | ₹139        | $1.53       | [Link](https://www.amazon.in/Electronicspices-Digital-Helicopter-Airplane-Controls/dp/B08XZQY94P) |
| 6        | Breadboard & jumpers| —                             | ₹199        | $2.19       | [Link](https://www.amazon.in/ApTechDeals-Breadboard-point-jumper-wires/dp/B07PQS67BN) |
| 7        | Resistors          | 10k ohm                        | ₹129        | $1.42       | [Link](https://www.amazon.in/10k-Ohm-Resistor-Tolerance-Pack/dp/B0DQFKBHBB) |
| 8        | Resistors          | 4.7k ohm                       | ₹129        | $1.42       | [Link](https://www.amazon.in/4-7k-Ohm-Resistor-Tolerance-Pack/dp/B0DQFHLBJ9) |
| 9        | PushButton         | --                             | ₹185        | %2.2        | [Link](https://www.amazon.in/ElectroBot-Momentary-Tactile-Push-Button/dp/B07PRRRBRY)
| **Total** | —                  | —                              | **₹2,611.87** | **$28.73** | — |

Note* In some of the links their are multiple component because I coudnt find single component link.
