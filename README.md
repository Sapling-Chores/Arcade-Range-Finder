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
