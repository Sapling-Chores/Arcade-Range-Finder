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
|3| UltraSonic Module | HC-SR04 Ultrasonic Module | ₹190 | | crid=14U9DTIS04OP8&dib=eyJ2IjoiMSJ9.f_xQWQlyPreKASwGL8luEksDL_qAUBuyNTUfKjF_OfD8dUBLwYTtRn2_J9lMyGqQjEsMO39317iB0qYUSr81h6Rme0LppQg6Nb4Qnymap5FLMP4ZFfVbUo13hmVH2SzbmnbkS8zKhJKeFuJrh3QvICnnTvPR0WZxtb8GXaVmy6qPlzypU6yUtv6S7R0rFZR5N-4vecUUbyIS-XKrzdAApf02K5QvFUwMlny5IS48vNkqxDXauEbd_7fAezgnB2OYSoBBEx2qTF48Ek0PSah3HwO8snNKg3R364alY-fuM8E.wRdafUbUPcDx9n4hSM1HebyCgHoQKoYIJZ1iEs4knQY&dib_tag=se&keywords=ultrasonic+sensor&qid=1768917669&s=|
|4| PotentioMeter | 10k 3Pin | ₹111 | | https://www.amazon.in/Electronic-Spices-Potentiometer-Multiple-Applications/dp/B0CP9NNMH3/ref=sr_1_5?crid=24M5VBI8ZBCNX&dib=eyJ2IjoiMSJ9.guAcVUOpF98GNdnuYG9n3NA85ytJ9XHxKUfhVN9H0imsjCp45QB42EDW1djEp0ZRZMBNYhToK6Z8NE8tHrh1nZLoPj3nVeMJ3L-eKtNMpijUQtOz8NL3iQjqAEvVNb5Tgui-LHQvh646jTrnLROxaqyyxnjzdjfrPYAw63uxNJmlpwtAKZrhC6jTgPFrnpn43MahJFxRrYNNd2xyyrzHtiP7nRjXfGId58trj5xEuHuqw3OC9Zyxu7wNELds8uV4nQRJe6JN1xgA9Bsfw7QV_mWZkOUOekh_Tk67QTheBVc.mUEehQgMmoaXbKV5MB-o_C4z2WlK0XJcJkv2EDzRx78&dib_tag=se&keywords=potentiometer&qid=1768917718&s=industrial&sprefix=potentiome%2Cindustrial%2C514&sr=1-5 |
|5| Servo Motor | SG90 Micro | ₹139 | | https://www.amazon.in/Electronicspices-Digital-Helicopter-Airplane-Controls/dp/B08XZQY94P/ref=sr_1_4?crid=1BYJSHX2ULWZO&dib=eyJ2IjoiMSJ9.sC6xGDPK02vC6q8e5uDqOgFgmyeQQIw98FEEc6OXvhsjR_DTbbHfVNuzjMiOBa1dU0LAy3QixTQgpwYuEbo0NJxX_LeUolSO0QuX2G47Qqi9Nd7kBqWI7DsNGtno4WnrLRJSUu8VK5d-c6HWCy2hkp0W8gg1kzAkeCpAfZfnvvfDtXwxt084HDdJwnaSU3TNRXjlRbAOFN9qX6bspAPD7S_7qTFDTybFRaBcJMYSzQIL_ASQoIkZMDENulfijitc2sPUBhIfLDMbzx1NNodeJ9v94jzflSgyWRZyXV9_V7M.7-Jr56vZ23duv8snFys2o-aiASdnC3HFagRboq8YbIc&dib_tag=se&keywords=servo&qid=1768917789&s=industrial&sprefix=ser%2Cindustrial%2C527&sr=1-4&th=1 |
|6| BreadBoard and jumpers| | ₹199 | | https://www.amazon.in/ApTechDeals-Breadboard-point-jumper-wires/dp/B07PQS67BN/ref=sr_1_3?crid=WMQ0RIZU817W&dib=eyJ2IjoiMSJ9.90gKDzZV_VCdozK0sQaNgx_2ybPDtWcO8UEjm0dh3IwyEGRMTj5YHlIEU9oVPy0ekXP22Cgx7Y8jt18iZi4fhlnDaewpjECG91JntCq1v_-jHi1ZWwD8InCReJijxQ0_47g1vQ0Uij0FI32KTSTEtQw_Iq7LNpNO7EW8rDfQrk_RZ5bDIemYLdm-QJQPvVZKxnnph8TO39feriWeOw8l0M_RvUsf-0MRyzPBZ0BEKtaMZW0lPr0MZClRDrGA5Or29_FoppNhRuLSz84TgruNUKdyximdW-rMRH4TB0rYGN0.vWdey3jsiSQQfdTHAtGbZIgxgIGCPC8U_hYiqhnl0b0&dib_tag=se&keywords=breadboard&qid=1768917931&refinements=p_n_g-101014971069111%3A206270883031&rnid=206270882031&s=industrial&sprefix=Bread%2Cindustrial%2C470&sr=1-3&th=1 |
|7| Resistors | 10k ohm | ₹129 | | https://www.amazon.in/10k-Ohm-Resistor-Tolerance-Pack/dp/B0DQFKBHBB/ref=sr_1_3?dib=eyJ2IjoiMSJ9.OjZigzBlGhN2l53skuBm4-qSmYUHwjQEtyLPOP7s0MGZeNOeaDmQnC7HgcrdqMBthexlJus4njlXua6ap8j_ga3A4PelqsJRK7BuwvwUhqQwYwa6iZuMdr2Teg9oKHnv0S_WNjbUT7bcWr2Z9_FP6hJzrHzcbHCeTKixvAcOtwXgaxnAY6Y1IUAWE5Az3GU04iHwbl-xGMEtvmvQ647JIyKFdZ0JuAvVvzm38Ls-jPi9diJMxcivT5JQT0r5d-wVp0VVi7kfzxWKOFmqHeWqPdqtdJ2f5_uaI28NSJXrivc.E9QQeF5Eee2AUSCSlBxs_49IwI6OQOz3RMUs30lfGNg&dib_tag=se&keywords=10k%2Bohm%2Bresistor&qid=1768918061&s=industrial&sr=1-3&th=1 | 
