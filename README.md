# RISC-V-Tapeout-RTL-to-GDSII-Week-2
The RISC-V Reference SoC Tapeout Program is a 20-week hands-on course guiding participants from RTL design to fabricated silicon. It covers synthesis, physical design, timing sign-off, verification, and chip validation using a 180 nm process. This week we get used to SoC reset, wavk-up and data flow.

🧠 Open-Source System-on-Chip (SoC) — RVMYTH Based

Sky130-based educational SoC built around the RVMYTH RISC-V core, integrating key digital and analog subsystems for learning, experimentation, and mixed-signal design exploration.

⚙️ Core Components
RVMYTH CPU Core

Simple RISC-V processor implementing base integer instructions.

Manages booting, configuration, interrupts (ISR), and data transfer via DMA.

Acts as the main control and computation engine of the SoC.

Phase-Locked Loop (PLL)

Generates and stabilizes the system clock.

Supports clock multiplication/division (e.g., 50 MHz → 500 MHz).

Reduces clock jitter and synchronizes multiple domains.

10-bit DAC (Digital-to-Analog Converter)

Converts digital values to analog voltages for real-world interfacing.

Equation: Vout = (D / (2^10 - 1)) × Vref

Supports R–2R Ladder DAC architecture (efficient for 10-bit resolution).

🧩 Subsystems Overview
Subsystem	Function
Memory	SRAM (on-chip cache/registers), DRAM (external main memory), ROM (boot code).
I/O Ports	GPIO, UART, SPI, I²C, and analog I/O for sensor & actuator interfacing.
GPU	Handles 2D/3D rendering and parallel compute workloads.
DSP	Performs high-speed signal processing (audio, video, communication).
PMU	Manages voltage, frequency (DVFS), and power gating for energy efficiency.
🌐 Special Features

Wireless Connectivity: Wi-Fi, Bluetooth, GNSS.

Security Modules: Crypto engine, Secure Boot, TEE.

Multimedia Engines: ISP, VPU, Audio DSP.

AI/ML Accelerators: Neural and tensor compute support.

Peripheral Interfaces: USB, PCIe, MIPI, SDIO, Ethernet.

🧩 SoC Type Classification

Microcontroller SoC: Low-power, embedded control.

Microprocessor SoC: Multi-tasking, OS-based systems.

Application-Specific SoC: Graphics, AI, or network-optimized chips.

💡 Project Summary — VSDBabySoC
Block	Description
CPU	RVMYTH RISC-V Core
PLL	8× Clock Multiplier
DAC	10-bit Digital-to-Analog Converter

Goal: A fully open-source, educational SoC platform demonstrating CPU–PLL–DAC integration using Sky130 technology.

Repository Purpose:
To serve as a learning reference for SoC architecture, digital–analog co-design, and open-source silicon workflows.
