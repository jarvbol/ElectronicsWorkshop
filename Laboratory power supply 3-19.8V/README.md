#  Adjustable Laboratory Power Supply (3V – 19.8V / 0 – 3.15A)

A compact, fully assembled bench-mounted power supply designed for prototyping and testing electronic circuits. It is equipped with precision voltage and current control, digital feedback. It is housed in a special case printed on a 3D printer.

![Power Supply Front View](./photo/3.jpg)
*Final assembly with OLED display and potentiometers*

---

##  Features

- **Voltage Range**: 3.0 V – 19.8 V (adjustable in 0.1V steps)
- **Current Limit**: Up to 3.15 A
- **Digital Monitoring**: Real-time voltage and current readout via OLED display (128x64, I2C)
- **Control Interface**: Two potentiometers  for precise adjustment
- **Feedback & Protection**: INA219 sensor for accurate current and bus voltage measurement
- **Enclosure**: Custom-designed 3D-printed case (PLA), ergonomic layout, and aesthetic finish
- **Regulation**: Based on LM2596-based DC-DC buck converter module with stable output

---

##  Hardware Components

| Component | Purpose |
|---------|--------|
| LM2596 Buck Converter Module | Voltage regulation |
| Arduino Nano | UI control, encoder input, display output |
| INA219 Sensor | Current and voltage monitoring |
| 128x64 OLED Display | Output visualization |
| 2x Rotary Encoders | User input for voltage/current adjustment |
| Tactile Buttons | Mode switching and confirmation |
| 3D-Printed Case | Mechanical housing and protection |

> All components are off-the-shelf or commonly available in hobbyist electronics stores.

---

##  Design Files

- **Schematic**: [`schematic.pdf`](./schematic.pdf) — Full circuit diagram
- **PCB Layout**: [`pcb_layout.png`](./pcb_layout.png) — Internal wiring and connections
- **3D Model**: Available for download on [Cults3D](https://www.cults3d.com/en/3d-model/various/power-supply-case) — Designed in Fusion 360

---

##  Assembly Photos

| ![Inside View](./photos/inside.jpg) | ![Display Close-up](./photos/display.jpg) | ![Working Demo](./photos/demo.jpg) |
|:---:|:---:|:---:|
| Internal wiring and component layout | OLED interface during operation | Powering a test load |

---

##  How It Works

1. The user adjusts the target voltage using the left rotary encoder.
2. The Arduino sends a PWM or analog signal to the LM2596 module to set the output.
3. The INA219 continuously measures actual voltage and current.
4. Values are displayed on the OLED screen in real time.
5. Over-current protection can be implemented in software (optional).

The system operates in a closed loop, ensuring stable and safe power delivery.

---

##  Usage Tips

- Always double-check polarity before connecting a load.
- Calibrate the INA219 sensor for accurate readings.
- Use thick enough wires for high-current applications (>2A).
- Ensure proper ventilation — the buck converter generates heat under load.

---

##  License

This project is open-source and licensed under the **MIT License**.  
See the [LICENSE](../../LICENSE) file in the root repository for details.

You are free to use, modify, and distribute the design, provided you include attribution.

---

