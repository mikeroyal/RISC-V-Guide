<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/102273505-43201980-3ed7-11eb-8b55-842f87faede4.png">
  <br />
  RISC-V Guide
</h1>

#### A guide covering the RISC-V Architecture including the applications, libraries and tools that will make you a better and more efficient developer with the RISC-V ISA.

**Note: You can easily convert this markdown file to a PDF in [VSCode](https://code.visualstudio.com/) using this handy extension [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf).**

# Table of Contents

1. [Models of RISC-V boards](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#models-of-risc-v-boards)

2. [RISC-V Learning Resources](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#risc-v-learning-resources)

3. [RISC-V Operating Systems](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#risc-v-operating-systems)

4. [RISC-V Tools](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#risc-v-tools)


<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/111917667-8b068d80-8a3e-11eb-9c0d-5ca40c81eb57.jpeg">
</p>

# Models of RISC-V boards

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

[Checkout the HiFive Unmatched Developement board](https://www.sifive.com/boards/hifive-unmatched)

<img src="https://user-images.githubusercontent.com/45159366/104135527-ea149b80-5345-11eb-902a-f07b7bd0b99b.png">

**HiFive Unmatched Hardware Specs**

**SoC:** SiFive Freedom U740 SoC

**Memory:** 16GB DDR4

**Flash Memory: ** 32MB Quad SPI Flash

**Removable Storage:** MicroSD Card

**Networking:** Gigabit Ethernet Port

**User I/O**

 - 4x USB 3.2 Gen 1 Type A Ports (1 Charging Port)

 - 1x MicroUSB Console Port

**Expansion Capabilities**

 - x16 PCIe® Gen 3 Expansion Slot (8-lanes Useable)

 - M.2 M-Key Slot (PCIe Gen 3 x4) for NVME 2280 SSD Module

 - M.2 E-Key Slot (PCIe Gen 3 x1) for Wi-Fi / Bluetooth Module

**Board Form Factor:** Industry Standard Mini-ITX


[Checkout the HiFive1 Rev B Developement board](https://www.sifive.com/boards/hifive1-rev-b)

<img src="https://user-images.githubusercontent.com/45159366/104135528-eb45c880-5345-11eb-8e47-22acd5a90e01.jpg">

**HiFive1 Rev B Hardware Specs**

**Microcontroller:** [FE310-G002](https://sifive.com/chip-designer#fe310)

**Operating Voltage:** 3.3 V and 1.8 V

**Input Voltage:** 5 V USB or 7-12 VDC Jack

**IO Voltage:** 3.3 V

**Digital I/O Pins:** 19

**PWM Pins:** 9

**SPI Controllers/HW CS Pins:** 1/3

**UART:** 2

**I2C:** 1

**Networking:** WiFi/BT (off-chip)

**External Interrupt Pins:** 19

**External Wakeup Pins:** 1

**Flash Memory:** 32 Mbit Off-Chip (ISSI SPI Flash)

**Host Interface (microUSB):** Program, Debug, and Serial Communication


[Checkout the Sipeed Maixduino Kit for RISC-V AI + IoT](https://www.seeedstudio.com/sipeed-maix.html)

[MAIX AI module](https://www.seeedstudio.com/Sipeed-MAIX-I-module-WiFi-version-1st-RISC-V-64-AI-Module-K210-inside-p-3206.html)

<img src="https://user-images.githubusercontent.com/45159366/104135531-ed0f8c00-5345-11eb-9c7d-d77f97bc16d5.jpeg">


**Sipeed Maixduino Kit Hardware Specs**

 - **CPU:** RISC-V Dual Core 64bit, with FPU; 400MHz neural network processor

 - QVGA@60FPS/VGA@30FPS image identification

 - Onboard ESP32 module support 2.4G 802.11. b/g/n and Bluetooth 4.2

 - [Arduino Uno](https://store.arduino.cc/usa/arduino-uno-rev3) form factor, Arduino compatible interface

 - Onboard omnidirectional I2S digital output MEMS Microphone

 - 24P 0.5mm FPC connector for DVP Camera

 - 8-bit MCU LCD 24P 0.5mm FPC connector

 - Support self-elastic micro SD card holder
 
 - High performance microphone array processor for machine hearing
 
 - Support MaixPy IDE, Arduino IDE, OpenMV IDE, and PlatformIO IDE
 
 - Support Tiny-Yolo, Mobilenet and TensorFlow Lite for deep learning
 
 
[Checkout the RTG4 Development Kit board from Microsemi](https://www.microsemi.com/product-directory/dev-kits-solutions/3865-rtg4-kits)

 <img src="https://user-images.githubusercontent.com/45159366/104135532-ee40b900-5345-11eb-9830-f57fe6d94f6f.jpeg">


**RTG4 Development Kit Hardware Specs**

 - Two 1GB DDR3 synchronous dynamic random access memory (SDRAM)
 
 - 2GB SPI flash memory
 
 - PCI Express Gen 1 x1 interface
 
 - PCIe x4 edge connector
 
 - One pair SMA connectors for testing of the full-duplex SERDES channel

 - Two FMC connectors with HPC/LPC pinout for expansion

 - RJ45 interface for 10/100/1000 Ethernet
 
 - USB micro-AB connector

 - Headers for SPI, GPIOs

 - FTDI programmer interface to program the external SPI flash

 - JTAG programming interface
 

# RISC-V Learning Resources

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)


[RISC-V Foundation](https://riscv.org/) is a non-profit corporation controlled by its 500 members(NVIDIA, Google, Samsung, Raspberry Pi, SiFive, Canonical, and Western Digital) to drive forward the adoption and implementation of the free and open RISC-V instruction set architecture (ISA).

[SiFive](https://www.sifive.com/) is a semiconductor company that produces complete RISC-V processors IP with pre-integrated SiFive Shield, for whole SoC security, and SiFive Insight advanced trace and debug. 

[IAR Systems](https://www.iar.com/) is a company that enables Linux-based Continuous Integration and automated workflows for embedded systems(ARM & RISC-V).

[The RISC-V Instruction Set Manual](https://riscv.org/wp-content/uploads/2019/12/riscv-spec-20191213.pdf)

[RISC-V Cores and SoC Overview](https://riscv.org/risc-v-cores/)

[Optimizing OpenCV for the RISC-V Architecture](https://opencv.org/optimizing-opencv-for-the-risc-v-architecture/)

[Software development kits, Toolchains and Utilities for RISC-V devices](https://www.sifive.com/software)

[RISC-V Development Board and RISC-V CPU](https://risc-v.ca)

[RISC-V CPUs from Microsemi](https://www.microsemi.com/product-directory/mi-v-risc-v-ecosystem/4406-risc-v-cpus#overview)

[RISC-V Community](https://riscv.org/community/)

[RISC-V Main Members Group](https://lists.riscv.org/g/main)

[RISC-V Global Forum](https://events.linuxfoundation.org/riscv-global-forum/)

[RISC-V Learn Online Courses](https://riscv.org/community/learn/risc-v-learn-online/)

[RISC-V Training Partner Program](https://riscv.org/exchange/training-partner-program/)

[SiFive Academy RISC-V Course](https://www.sifiveacademy.com/)

[Risc-V Courses on Udemy](https://www.udemy.com/topic/risc-v/)

[Imagination Technologies Announces the First RISC-V Computer Architecture Course](https://riscv.org/news/2020/09/imagination-announces-the-first-risc-v-computer-architecture-course/)

[RISC-V Design Verification Strategy](https://verificationacademy.com/verification-horizons/november-2020-volume-16-issue-3/risc-v-design-verification-strategy)

# RISC-V Operating Systems

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

[RISC-V - Ubuntu Wiki](https://wiki.ubuntu.com/RISC-V)

<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/106686328-f5db3280-657e-11eb-9109-88a1df99983a.png">
  <br />
</h1>

[RISC-V - Kubuntu Wiki](https://wiki.kubuntu.org/RISC-V)

<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112046427-40057c80-8b09-11eb-856f-9233f55d691f.png">
  <br />
</h1>

[RISC-V - Debian Wiki](https://wiki.debian.org/RISC-V)

<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/107439775-73ef8a00-6ae7-11eb-9037-6aa910fc3c74.png">
  <br />
</h1>

[RISC-V - Fedora Project Wiki](fedoraproject.org/wiki/Architectures/RISC-V)

<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/107158827-70220300-6941-11eb-917b-dbdb7142a13b.png">
  <br />
</h1>


[RISC-V - openSUSE Wiki](https://en.opensuse.org/openSUSE:RISC-V)

<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/110253145-a00ef700-7f3d-11eb-9b5c-d3cee3cbce84.png">
  <br />
</h1>

[SUSE Wiki](https://documentation.suse.com/)

 <h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/110253144-9f766080-7f3d-11eb-9a01-2ac6738637e9.png">
  <br />
</h1>

[Manjaro ARM](https://wiki.manjaro.org/index.php/Manjaro-ARM)

 <h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/110054438-f3036700-7d0f-11eb-88bc-dab9b262c097.png">
  <br />
</h1>

[EndeavourOS Wiki](https://endeavouros.com/wiki/)

<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/107439882-9e414780-6ae7-11eb-819e-e87e7bcc7a97.png">
  <br />
</h1>

[Zephyr OS](https://www.zephyrproject.org/zephyr-rtos-featured-in-risc-v-getting-started-guide/) is a popular security-oriented RTOS with a small-footprint kernel designed for use on resource-constrained and embedded systems. Zephyr has a small-foorprint Kernel focusing on embedded devices compatible with x86, ARM, RISC-V, Xtensa and [others](https://docs.zephyrproject.org/latest/boards/index.html).

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112046437-4267d680-8b09-11eb-958d-7a5875f6593a.png">
</p>


## RISC-V Tools

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

[Ashling RiscFree™ C/C++ for RISC-V](https://www.sifive.com/software) is a fully integrated development tool environment that includes an IDE, compiler, debugger, and Opella-XD JTAG probe ready to use with SiFive's RISC-V Core IP products. 

[RISCVEMU](https://riscv.org/software-tools/riscvemu/) is a system emulator developed by Fabrice Bellard for the RISC-V architecture. Its purpose is to be small and simple while being complete. Among its features are the support of 128 bit addressing and 128 bit floating point which makes the emulator ready for the future.

[RISC-V Interpreter](http://www.cs.cornell.edu/courses/cs3410/2019sp/riscv/interpreter/) is a online Interpreter for RISC-V build by Cornell University.

[Chipyard](https://chipyard.readthedocs.io/en/latest/) is an open source framework for agile development of Chisel-based systems-on-chip. It will allow you to leverage the Chisel HDL, Rocket Chip SoC generator, and other [Berkeley](https://berkeley.edu/) projects to produce a RISC-V SoC with everything from MMIO-mapped peripherals to custom accelerators.

[The Eclipse Embedded CDT](https://github.com/eclipse-embed-cdt/eclipse-plugins) is a collection of plug-ins for Arm & RISC-V C/C++ developers.

[PlatformIO](https://platformio.org/) is a professional collaborative platform for embedded development with no vendor lock-in. It provides support for multiplatforms and frameworks such as IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbed OS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V.

[PlatformIO for VSCode](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) is a plugin that provides support for the PlatformIO IDE on VSCode.

[Ripes](https://github.com/mortbopet/Ripes) is a graphical processor simulator and assembly editor for the RISC-V instruction set architecture(ISA).

[FireSim](https://github.com/firesim/firesim) is an easy-to-use, Scalable, FPGA-accelerated Cycle-accurate Hardware Simulation.

[Tock](https://www.tockos.org/) is an embedded operating system designed for running multiple concurrent, mutually distrustful applications on Cortex-M and RISC-V based embedded platforms. Tock's design centers around protection, both from potentially malicious applications and from device drivers. 

[TinyGo](https://tinygo.org/) is a Go compiler(based on LLVM) intended for use in small places such as microcontrollers, WebAssembly (Wasm), and command-line tools.

[LLVM](https://github.com/llvm/) is a library that has collection of modular/reusable compiler and toolchain  components (assemblers, compilers, debuggers, etc.). With these components LLVM can be used as a compiler framework, providing a front-end(parser and lexer) and a back-end (code that converts LLVM's representation to actual machine code).

[Unicorn](https://github.com/unicorn-engine/unicorn) is a lightweight, multi-platform, multi-architecture CPU emulator framework(ARM, AArch64, M68K, Mips, Sparc, X86) based on [QEMU](https://www.qemu.org/).

[Keystone](https://github.com/keystone-engine/keystone) is a lightweight multi-platform, multi-architecture(Arm, Arm64, Hexagon, Mips, PowerPC, Sparc, SystemZ & X86) assembler framework.

[Reko](https://github.com/uxmal/reko) is a decompiler for machine code binaries.

[Renode](https://renode.io/) is [Antmicro's](https://antmicro.com) virtual development framework for multinode embedded networks (both wired and wireless) and is intended to enable a scalable workflow for creating effective, tested and secure IoT systems.

[Jupiter](https://jupitersim.gitbook.io/) is an open source and education-oriented RISC-V assembler and runtime simulator written in Java.

[RISC-V Rust](https://github.com/takahirox/riscv-rust) is a RISC-V processor and peripheral devices emulator project written in Rust and compiled to WebAssembly.

[Diosix](https://diosix.org/) is a lightweight, secure, multiprocessor bare-metal hypervisor written in Rust for RISC-V.

[Maixpy](https://maixpy.sipeed.com/) is designed to make AIOT programming easier with Micropython running on the embedded AIOT chip [K210](https://kendryte.com/).

[DarkRISCV](https://github.com/darklife/darkriscv) is an open souce RISC-V cpu core implemented in Verilog from scratch.

## Contribute

- [x] If would you like to contribute to this guide simply make a [Pull Request](https://github.com/mikeroyal/RISC-V-Guide/pulls).


## License
[Back to the Top](https://github.com/mikeroyal/RSIC-V-Guide/blob/master/README.md#table-of-contents)

Distributed under the [Creative Commons Attribution 4.0 International (CC BY 4.0) Public License](https://creativecommons.org/licenses/by/4.0/).
