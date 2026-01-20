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

|Item no.| Component | Specs/Model | Price(inr) | print(US$) | Item link |
|--------|---------|----------|----------|----------|-----------|
|1| Esp32 devkit | ESP32-S3-DevKitC-1-N8R8 | ₹1,194.87 |  | https://www.mouser.in/ProductDetail/Espressif-Systems/ESP32-S3-DevKitC-1-N8R8?qs=7D1LtPJG0i2PiuUUKucutQ%3D%3D&mgh=1&utm_source=chatgpt.com |
|2| Oled display| SSD1306 Oled 128x64 | ₹520 | |  https://www.amazon.in/Robocraze-Inches-Display-Module-Arduino/dp/B077TH5WWY/ref=sr_1_4?dib=eyJ2IjoiMSJ9.vbp0qyzflQP5BctmfwNQWfvfq5d0rBffZLTCgsKJsotCp-RSxjECm4ZzC5Qr7csc9YKgzLwX53eAiJhzrc7RiguvxnZgVFEZAtWrT_CghX__2SArG8rZaw5rv5tfhZh6E-giAbKS8T9CbTFWcgmloV06WaKYFYIlYPa-LxdQdH7qB53pf4l_NVCYakRcpbFnDUDvsQJCtrm-rqLmwUQ7Nvp4dZcjhdEkp53VtxkaSBRtd4ELyUdC7estNk84_U6xIg7d1FqqEKXMkQFjbF8_glVYY_bRO0JB7UXQmB2VI8M.14siSUgOqSVQMm6OfyX8ZF7PUsEESOzVr0kLCd-rvuI&dib_tag=se&keywords=ssd1306%2Boled%2Bdisplay&qid=1768917563&sr=8-4&th=1|
