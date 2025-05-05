# Arduino Radar System

This project simulates a basic radar system using an Arduino UNO, an ultrasonic sensor, a servo motor, LEDs, and a buzzer. The sensor scans the surrounding area and detects objects based on distance. The output is visualized through LEDs, sound alerts, and an optional radar-like interface using the Processing IDE.

---

## 🔧 Components Used

| # | Component                  | Description                         | Specs / Notes                                 |
|---|----------------------------|-------------------------------------|------------------------------------------------|
| 1 | Arduino UNO               | Microcontroller board               | AVR/ARM CPU, Flash + SRAM, open-source        |
| 2 | HC-SR04 Ultrasonic Sensor | Distance measurement via sound      | Range: 2–400 cm, Accuracy: ±3 mm              |
| 3 | 9G Micro Servo            | Rotates sensor for scanning         | Angle: 0°–180°, Controlled by PWM             |
| 4 | Buzzer                    | Audio alert for object detection    | Beeps when object detected within threshold   |
| 5 | Resistors (1KΩ, 220Ω ×4)  | Protects components                 | 1KΩ: Signal control, 220Ω: For LEDs           |
| 6 | Breadboard                | Circuit assembly platform           | Solderless, reusable                          |
| 7 | Jumper Wires (×25)        | Connects components                 | Male-to-male, flexible prototyping            |
| 8 | USB Cable (A/B)           | Uploads code to Arduino             | For power and data                             |
| 9 | Red LEDs (×2)             | Warning indicators                  | Indicate system and object detection status   |
| 10| Green LED                 | Status indicator                    | Glows when radar is active                    |
| 11| Slide Switch              | Power toggle                        | Controls circuit ON/OFF                       |

---

##  How It Works

- The **ultrasonic sensor** sends sound waves and detects objects based on echo timing.
- The **servo motor** moves the sensor from side to side (0°–180°).
- When an object is detected:
  - **Red LED** blinks
  - **Buzzer** sounds
  - Data is sent to a radar-like visual on the **Processing IDE** (optional).
- A **slide switch** turns the radar system on and off.
- **Green LED** shows when the system is actively scanning.

---

## 🛠️ Setup Instructions

1. Install [Arduino IDE](https://www.arduino.cc/en/software) and [Processing IDE](https://processing.org/download).
2. Wire components as per the circuit diagram.
3. Upload Arduino code via USB.
4. Open Processing IDE and adjust:
   - Line 24: Set display resolution
   - Line 26: Set correct COM port
5. Run both sketches to start the radar system.
