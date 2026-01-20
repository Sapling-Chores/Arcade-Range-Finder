# Wiring

## ESP32 Pin Connections

### HC-SR04
| ESP32 Pin | HC-SR04 Pin |
|-----------|------------|
| ---        | Vcc        |
| GND       | GND        |
| GPIO 2    | TRIG       |
| GPIO 4    | ECHO       |

### Potentiometer (10k)
| ESP32 Pin | Potentiometer Pin |
|-----------|-----------------|
| 3.3v        | 5V              |
| GND       | GND             |
| GPIO 36 / A0 | Signal (A0)   |

### SG90 Servo
| ESP32 Pin | SG90 Pin |
|-----------|----------|
| ---       | PWR      |
| GND       | GND      |
| GPIO 16   | SIG      |

### Buzzer
| ESP32 Pin | Buzzer Pin |
|-----------|------------|
| GPIO 17   | +          |
| GND       | -          |

### Push Buttons
| ESP32 Pin | Button |
|-----------|--------|
| GPIO 18   | S1     |
| GPIO 19   | S2     |

### Pull-up / Pull-down Resistors
- **R1 (10Ω)**: Series with sensor signals if needed.
- **R2 (4.7kΩ)**: Pull-up on buttons if configured as active-low.

## Wiring Diagram Notes
1. All grounds (GND) **must be common**.
2. Signal pins (TRIG, ECHO, SIG) go to **ESP32 GPIO** pins as defined.
3. Use short wires for accurate ultrasonic sensor readings.
4. Push-buttons can use **internal pull-ups** in ESP32 software.
