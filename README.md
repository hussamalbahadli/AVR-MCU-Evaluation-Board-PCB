# AVR MCU Evaluation Board — PCB

A full-featured development and training board for the **ATmega32 / ATmega16**, designed in **Altium Designer**.
It puts the peripherals a student or developer needs to learn embedded C on one board — displays, communication interfaces, sensors, motor drivers and an on-board USB programmer — so every exercise runs on real hardware without breadboard wiring.

> Firmware for this board (drivers, examples and Proteus simulations) lives in
> **[AVR-MCU-Evaluation-Board-DES](https://github.com/hussamalbahadli/AVR-MCU-Evaluation-Board-DES)**.

![Top view](Doc/Image/AVR%20MCU%20Evaluation%20Board%20Above.png)

---

## 01. Specifications

| Item | Value |
|---|---|
| MCU | ATmega32 / ATmega16 (DIP-40, socketed) |
| Board size | 230 × 200 mm |
| Layers | 2 |
| Holes | 1187 plated through-holes |
| Power input | 7.5 V DC jack |
| Regulators | LM7805 (5 V) + LM317 (adjustable) |
| Programming | On-board USB programmer + 10-pin ISP header |
| Design tool | Altium Designer 24 |

---

## 02. On-board peripherals

| Group | Peripherals |
|---|---|
| Displays | 16×2 character LCD · graphical LCD header · 4-digit multiplexed 7-segment · 8 LEDs · RGB LED |
| Inputs | 4 push buttons · 4×4 keypad · DIP switches with selectable pull-up / pull-down |
| Communication | USART over RS232 (MAX232, DB9) · RS485 (ADM485) · SPI · I²C |
| Memory & time | AT24C04 I²C EEPROM · DS1307 real-time clock with coin-cell backup · MMC/SD connector |
| Analog & sensors | LM35 temperature sensor · infrared transmitter/receiver (LM358) · MCP41010 SPI digital potentiometer |
| Actuators | Relay · buzzer · stepper motor driver (ULN2003) · DC motor driver (L298) |
| Other | CD4046 PLL · external clock section · reset circuit |
| Expansion | All MCU ports broken out on labelled headers · prototyping area |

---

## 03. Board views

| Top — with components | Top — bare board |
|---|---|
| ![](Doc/Image/AVR%20MCU%20Evaluation%20Board%20Above.png) | ![](Doc/Image/AVR%20MCU%20Evaluation%20Board%20Above_2.png) |

| Bottom — with components | Bottom — bare board |
|---|---|
| ![](Doc/Image/AVR%20MCU%20Evaluation%20Board%20Bottom.png) | ![](Doc/Image/AVR%20MCU%20Evaluation%20Board%20Bottom_2.png) |

---

## 04. Manufacturing files

`Doc/Gerber/AVR MCU Evaluation Board.zip` contains everything needed to fabricate the board:

| File | Layer |
|---|---|
| `.GTL` / `.GBL` | Top / bottom copper |
| `.GTS` / `.GBS` | Top / bottom solder mask |
| `.GTO` / `.GBO` | Top / bottom silkscreen |
| `.GTP` / `.GBP` | Top / bottom paste |
| `.GM` | Board outline |
| `.TXT` | NC drill file |
| `.DRR` | Drill report |

The same package is attached to the **[v1.0.0 release](https://github.com/hussamalbahadli/AVR-MCU-Evaluation-Board-PCB/releases)**.

---

## 05. Status

| Item | Status |
|---|---|
| PCB design | Done (Dec 2024) |
| Fabrication | Done |
| Assembly | Pending |
| Schematic PDF | Planned |

---

## 06. Related repositories

- [AVR-MCU-Evaluation-Board-DES](https://github.com/hussamalbahadli/AVR-MCU-Evaluation-Board-DES) — drivers, examples and simulations for this board
- [STM32F7-MCU-Evaluation-Board-DES](https://github.com/hussamalbahadli/STM32F7-MCU-Evaluation-Board-DES) — the same driver architecture, ported to the STM32F746

---

## License

GPL-3.0 — see [LICENSE](LICENSE).
