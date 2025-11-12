#  Mini Soldering Station on the base Hanlei T12

A compact, custom-built soldering station based on the popular **Hanlei T12** controller board. Enhanced with a sleek acrylic enclosure, dedicated power input, and a physical power switch for improved usability and safety.

![Front View](./photo/front.jpg)
*Front panel with digital display, rotary encoder, and power connector*

---

##  Features

- **Core Controller**: Hanlei T12 (supports T12, JBC, TS100, and other cartridges)
- **Enclosure**: Custom laser-cut black acrylic case with precise cutouts and ventilation grid
- **Power Input**: Dedicated 5-pin XLR-style connector for stable DC power delivery
- **Power Switch**: Physical toggle switch for safe on/off control
- **Display**: Integrated 7-segment LED display for temperature readout
- **Control**: Rotary encoder with push-button for intuitive menu navigation
- **Ventilation**: Perforated back panel for heat dissipation during prolonged use

---

##  Hardware Modifications

This project is not just an assembly — it’s a **complete redesign of the user interface and mechanical housing**:

- Replaced the original plastic casing with a **custom-designed acrylic box**.
- Added a **dedicated power socket** to avoid using micro-USB for high-current applications.
- Installed a **latching power switch** for quick and safe shutdown.
- Designed a **ventilated rear panel** to prevent overheating of the controller board.
- All components are securely mounted using standoffs and screws for durability.

> This design prioritizes **safety**, **ergonomics**, and **long-term reliability** over the stock kit.

---

##  Design Files

- **3D Model / Laser Cut Plans**: Available for download on [Cults3D](https://cults3d.com/:3684383) — designed in QCAD

---

##  Assembly Photos

| ![Front Panel](./photos/front.jpg) | ![Back Panel](./photos/back.jpg) | ![Internal Layout](./photos/internal.jpg) |
|:---:|:---:|:---:|
| Power connector and display | Ventilated rear with rubber feet | Clean internal layout with secure mounting |

---

##  How It Works

1. The Hanlei T12 board controls the heating element via PID algorithm.
2. Temperature is displayed on the 7-segment LED.
3. User adjusts settings via the rotary encoder.
4. Power is supplied through the XLR connector and controlled by the front-panel switch.
5. Heat dissipates through the perforated back panel.

The station supports multiple tip types (T12, JBC, etc.) and can be calibrated for precise temperature control.

---

##  Usage Tips

- Always use a regulated DC power supply (recommended: 24V, 3A+).
- Avoid touching the heating element or tip during operation.
- Calibrate the temperature sensor for accurate readings.
- Clean the tip regularly with a damp sponge or brass wool.

---

##  License

This project is licensed under the **MIT License**.  
See the [LICENSE](../../LICENSE) file in the root repository for details.

You are free to use, modify, and distribute the design, provided you include attribution.
