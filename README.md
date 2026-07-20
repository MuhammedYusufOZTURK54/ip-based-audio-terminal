# IP-Based Audio Broadcasting and Control Terminal

An industrial-grade hardware design for an IP-based audio broadcasting and control terminal. This project was developed from end-to-end using **Altium Designer**, focusing on high-speed signal integrity, thermal management, and DFM/DRC industrial standards.

## Hardware Specifications
* **Main Microcontroller:** ESP32-WROOM-32E
* **Ethernet Controller:** WIZnet W5500 (Hardware TCP/IP)
* **Digital-to-Analog Converter (DAC):** PCM5102A (I2S Interface)
* **Audio Amplifier:** TPA3111D1 Class-D Stereo Amplifier (10-W)
* **Power Management:** Cascade topology with LM2940 (12V), LD1117 (5V), and AZ1117 (3.3V) linear regulators.

## Communication Interfaces
* **SPI:** High-speed communication between ESP32 and W5500 Ethernet controller.
* **I2S:** High-fidelity digital audio data transfer to the DAC.
* **SDIO:** Local storage integration via MicroSD card slot.
* **UART:** Integrated auto-programming circuit for the ESP32.

## PCB Design & Engineering Highlights
* **High-Speed Routing:** 100-ohm differential impedance matching and length tuning for W5500 and RJ45 isolation transformer connections.
* **Signal Integrity:** Maintained strict clearance rules and physical isolation between high-speed digital lines and analog layers to minimize crosstalk. 45-degree routing and teardrop supports were applied to prevent acid traps.
* **Production Ready:** Passed strict DRC (Design Rule Check) and DFM (Design for Manufacturing) guidelines.


## Repository Contents
* `Schematics/`: High-resolution PDF exports of the schematic designs.
* `PCB_Layout/`: 2D and 3D PDF views of the PCB routing and placement.
* `Manufacturing/`: Gerber X2, NC Drill, and ActiveBOM files ready for production.

---
*Designed by Muhammed Yusuf Öztürk*
