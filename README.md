# 🌐 uCompute Ecosystem — Central Documentation & Wiki

Welcome to the central repository for the **uCompute Ecosystem**, a fully open-source, modular, and interconnected hardware/software platform powered by the **Raspberry Pi RP2040 and RP2350** microcontrollers. 

This repository acts as the central umbrella wiki and documentation hub, bridging together all hardware designs, custom firmware configurations, and software stacks across the entire ecosystem. Whether you are a seasoned engineer looking for a surface-mount soldering challenge, a retro-computing enthusiast, or an educator setting up a STEM workshop in a Fablab, this ecosystem adapts to your needs.

---

## 🗺️ Ecosystem Overview & Core Projects

The ecosystem shares a common hardware DNA and is built around **uComputeOS** (a custom MicroPython visual GUI environment featuring runtime fault tolerance). It currently features 5 main hardware implementations, all fully open-source under the **CC BY-NC-SA 4.0** license:

*   **💻 [RP2040 uCompute](https://github.comRP2040_uCompute):** The foundation of the ecosystem. An autonomous, highly modular embedded development platform integrating extended storage (MicroSD, EEPROM), display options (IPS ST7789/OLED), and a versatile rear expansion socket for communication daughterboards.
*   **🚀 [RP2350 uCompute2](https://github.com/RP2350_uCompute2):** The next-generation evolution leveraging the raw hardware capabilities, security features, and expanded GPIO flexibility of the brand-new Raspberry Pi RP2350 chip.
*   **🎓 [uCompute Junior](https://github.comuComputeJr):** A "Bring Your Own Pico" educational variant. It lowers the barrier to entry by removing complex SMD microchip soldering, opting for comfortable 0805 components. Perfect for hand-soldering initiation in schools and Fablabs.
*   **🤖 [uCompute Rover](https://github.com/uCompute_Rover):** A modular 4WD robotic platform driven by the uCompute core. It interfaces seamlessly with dual bridge motor drivers, ultrasonic sensors, time-of-flight lasers, and GPS modules for both RC-controlled and 100% autonomous navigation.
*   **🕹️ [RetroPico (v1.x)](https://github.com/RetroPico_V1.x):** A pocket-sized (60mm x 45mm) retro-gaming and vintage video emulation motherboard. Features a native analog VGA output (configurable monochrome/3-bit RGB), audio buzzer, and full USB-Host support to connect standard keyboards or gamepads.

---

## 🔌 Shared Modular Architecture & Add-ons

One of the greatest strengths of the uCompute framework is its **backwards and cross-compatibility**. The standardized rear communication socket and front expansion headers allow daughterboards to be swapped seamlessly between different mainboards:
*   **Wireless Télémétry:** Plug-and-play modules for Wi-Fi (ESP-12F), short-range radio (nRF24L01+), and long-range telemetry (LoRa RFM95W).
*   **Inter-Chip Bus Stability:** Shared SPI and I2C lines optimized at the hardware level with precise pull-up configurations and logical separation.
*   **Smart IO Saving:** Proven hardware compromises, such as an analog resistor ladder configuration to sample multiple user buttons through a single ADC channel, freeing up digital GPIOs for critical high-speed buses.

---

## 📖 What You Will Find in This Wiki

This hub compiles comprehensive hardware and software guidelines, including:
1.  **Hardware Design & Assembly Checklists:** Deep dives into schematic choices, 0805 manual soldering tips, and critical safety rules (e.g., managing dual USB-C/USB-A alternative power lines to prevent reverse current loops to your PC).
2.  **Pinout & Memory Maps:** Comprehensive lookup tables detailing GPIO configurations and shared I2C addresses across all revisions.
3.  **uComputeOS Deployment:** Setup guides for MicroPython firmwares, compiling network drivers (W5500), managing standalone automated boots (`main.py`), and configuring AI Coding Assistant profiles (ChatGPT/Claude prompts) optimized with the exact board pinouts.
4.  **Community & Learning Resources:** Sample codes (`testcode/`), retro games, and step-by-step entry pathways matching official Raspberry Pi foundation tutorials.

---

## 📜 Philosophy & License

This entire ecosystem is a non-commercial, hobbyist initiative born out of a personal challenge to blend classic embedded hardware principles with modern, powerful microcontrollers. Everything is open-source and shared under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license. Commercial distribution of bare PCBs, pre-assembled kits, or commercial derivatives is strictly prohibited without prior authorization.

