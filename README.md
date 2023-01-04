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
     - [Developer Resources](https://github.com/mikeroyal/RISC-V-Guide#developer-resources)
     - [Learning/Training Courses](https://github.com/mikeroyal/RISC-V-Guide#learningtraining-courses)
     - [Books](https://github.com/mikeroyal/RISC-V-Guide#books)

3. [RISC-V Operating Systems](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#risc-v-operating-systems)
     * [Linux-based Operating Systems](https://github.com/mikeroyal/RISC-V-Guide#linux-based-operating-systems)
     * [BSD-based Operating Systems](https://github.com/mikeroyal/RISC-V-Guide#bsd-based-operating-systems)
     * [Real-Time Operating Systems (RTOS)](https://github.com/mikeroyal/RISC-V-Guide#real-time-operating-systems-rtos)
     * [seL4 Operating Systems](#seL4-Operating-Systems)

4. [RISC-V Tools](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#risc-v-tools)

5. [FPGA(Field Programmable Gate Arrays) Development](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#fpga-development)

6. [Verilog/SystemVerilog Development](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#verilogsystemverilog-development)

7. [Assembly Development](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#assembly-development)

8. [Telco 5G Development](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#telco-5g-development)

9. [Kubernetes](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#kubernetes)

10. [Machine Learning](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#machine-learning)

11. [Robotics](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#robotics)

12. [Networking](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#networking)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/121087082-d35d5e00-c798-11eb-94bb-58bf863bd724.png">
</p>

# Models of RISC-V boards

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

[Checkout the StarFive VisionFive 8GB RISC-V SBC](https://www.aliexpress.com/item/3256803492307592.html)

 <img src="https://user-images.githubusercontent.com/45159366/171485293-3988aea2-a6da-49bb-9e8d-0af066d1f229.png">
 
 **StarFive VisionFive Hardware Specs**
 
**CPU:** U74 Dual-Core with 2MB L2 cache, running at 1.0GHz. The SoC includes Vision DSP Tensilica-VP6 for computing vision at 600MHz (VPU), an NVIDIA  Deep Learning Accelerator, and a neural network engine.

**Memory:** 8GB LPDDR4 RAM (2x 4GB clocked at 2800MHz)

**User I/O**
- 4 x USB3.0 Ports, Gigabit Ethernet, Audio jack
- 40 Pin GPIO Header (28 x GPIO, I2C, I2S, SPI, UART)

**Networking:** Wi-Fi and Bluetooth 4.2

Linux Ready including **Fedora**.

[Checkout the HiFive Unmatched Developement board](https://www.sifive.com/boards/hifive-unmatched) **(Discontinued as of January 2022)**

<img src="https://user-images.githubusercontent.com/45159366/104135527-ea149b80-5345-11eb-902a-f07b7bd0b99b.png">

**HiFive Unmatched Hardware Specs**

**SoC:** SiFive Freedom U740 SoC

**Memory:** 16GB DDR4

**Flash Memory:** 32MB Quad SPI Flash

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
 
**[Checkout the Espressif ESP32-C3](https://www.espressif.com/en/products/socs/esp32-c3)**

[Espressif ESP32-C3](https://www.espressif.com/en/products/socs/esp32-c3) is a single-core Wi-Fi and Bluetooth 5 (LE) microcontroller SoC, based on the open-source RISC-V architecture. It has the right balance of power, I/O capabilities and security, thus offering the optimal cost-effective solution for connected devices. The availability of Wi-Fi and Bluetooth 5 (LE) connectivity not only makes the device's configuration easy, but it also facilitates a variety of use-cases based on dual connectivity.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177451635-64cda8af-b05f-4506-acc1-d9ddf5a894f1.png">
  <br />
</p>

**Espressif ESP32-C3 Hardware Specs:**

- 32-bit core RISC-V microcontroller with a maximum clock speed of 160 MHz. 
- 22 configurable GPIOs.
- 400 KB of internal RAM. 
- Low-power-mode support.
- RSA-3072-based secure boot.
- AES-128/256-XTS-based flash encryption.
- Wi-Fi and Bluetooth 5 (LE).

[Espressif ESP32-C3-DevKitC-02](https://docs.espressif.com/projects/esp-idf/en/latest/esp32c3/hw-reference/esp32c3/user-guide-devkitc-02.html) is an entry-level development board based on [ESP32-C3-WROOM-02](https://www.espressif.com/sites/default/files/documentation/esp32-c3-wroom-02_datasheet_en.pdf), a general-purpose module with 4 MB SPI flash. This board integrates complete Wi-Fi and Bluetooth LE functions.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177451653-b77a9819-2308-4080-b2dd-8aec755b5583.png">
  <br />
  ESP32-C3-DevKitC-02
</p>

[Espressif ESP32-C3-DevKitM-1](https://docs.espressif.com/projects/esp-idf/en/latest/esp32c3/hw-reference/esp32c3/user-guide-devkitm-1.html) is an entry-level development board based on [ESP32-C3-MINI-1](https://www.espressif.com/sites/default/files/documentation/esp32-c3-mini-1_datasheet_en.pdf), a module named for its small size. This board integrates complete Wi-Fi and Bluetooth LE functions.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177451647-4831fad4-8fc9-4c50-858f-dbb11c829df8.png">
  <br />
  ESP32-C3-DevKitM-1
</p>

# RISC-V Learning Resources

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)


[RISC-V Foundation](https://riscv.org/) is a non-profit corporation controlled by its 500 members(NVIDIA, Google, Samsung, Raspberry Pi, SiFive, Canonical, and Western Digital) to drive forward the adoption and implementation of the free and open RISC-V instruction set architecture (ISA).

[SiFive](https://www.sifive.com/) is a semiconductor company that produces complete RISC-V processors IP with pre-integrated SiFive Shield, for whole SoC security, and SiFive Insight advanced trace and debug. 

[IAR Systems](https://www.iar.com/) is a company that enables Linux-based Continuous Integration and automated workflows for embedded systems(ARM & RISC-V).

### Developer Resources
[Back to the Top](https://github.com/mikeroyal/risc-v-Guide#table-of-contents)

- [RISC-V Cores and SoC Overview](https://riscv.org/risc-v-cores/)

- [Optimizing OpenCV for the RISC-V Architecture](https://opencv.org/optimizing-opencv-for-the-risc-v-architecture/)

- [Software development kits, Toolchains and Utilities for RISC-V devices](https://www.sifive.com/software)

- [RISC-V Development Board and RISC-V CPU](https://risc-v.ca)

- [RISC-V CPUs from Microsemi](https://www.microsemi.com/product-directory/mi-v-risc-v-ecosystem/4406-risc-v-cpus#overview)

- [RISC-V Community](https://riscv.org/community/)

- [RISC-V Main Members Group](https://lists.riscv.org/g/main)

- [RISC-V Global Forum](https://events.linuxfoundation.org/riscv-global-forum/)

- [Porting Android onto RISC-V: Android 12 upgrade, vendor modules and TensorFlow Lite](https://riscv.org/blog/2022/07/progress-in-porting-android-onto-risc-v-android-12-upgrade-vendor-modules-and-tensorflow-lite-mao-han-alibaba-cloud/)

### Learning/Training Courses
[Back to the Top](https://github.com/mikeroyal/risc-v-Guide#table-of-contents)

- [RISC-V Learn Online Courses](https://riscv.org/community/learn/risc-v-learn-online/)

- [RISC-V Training Partner Program](https://riscv.org/exchange/training-partner-program/)

- [SiFive Academy RISC-V Course](https://www.sifiveacademy.com/)

- [Risc-V Courses on Udemy](https://www.udemy.com/topic/risc-v/)

- [Imagination Technologies Announces the First RISC-V Computer Architecture Course](https://riscv.org/news/2020/09/imagination-announces-the-first-risc-v-computer-architecture-course/)

 - [RISC-V Design Verification Strategy](https://verificationacademy.com/verification-horizons/november-2020-volume-16-issue-3/risc-v-design-verification-strategy)
 
 ### Books
 [Back to the Top](https://github.com/mikeroyal/risc-v-Guide#table-of-contents)
 
 - [The RISC-V Instruction Set Manual](https://riscv.org/wp-content/uploads/2019/12/riscv-spec-20191213.pdf)
 
 - [RISC-V Assembly Programmer's Manual](https://github.com/riscv-non-isa/riscv-asm-manual/blob/master/riscv-asm.md)
 
 - [Digital Design and Computer Architecture, RISC-V Edition](https://www.amazon.com/Digital-Design-Computer-Architecture-RISC-V/dp/0128200642)
 
 - [Computer Organization and Design RISC-V Edition (The Morgan Kaufmann Series in Computer Architecture and Design)](https://www.amazon.com/Computer-Organization-Design-RISC-V-Architecture/dp/0128203315)
 
 - [The RISC-V Reader: An Open Architecture Atlas ](https://www.amazon.ca/RISC-V-Reader-Open-Architecture-Atlas/dp/0999249118)
 
 - [An Introduction to Assembly Programming with RISC-V](https://riscv-programming.org/book.html)

 - [Digital Design with Chisel Book](https://github.com/schoeberl/chisel-book)

# RISC-V Operating Systems

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

* [Running 32-bit & 64-bit RISC-V Linux on QEMU](https://risc-v-getting-started-guide.readthedocs.io/en/latest/linux-qemu.html)

### Linux-based Operating Systems
[Back to the Top](#table-of-contents)

 * [RISC-V - Ubuntu Wiki](https://wiki.ubuntu.com/RISC-V)

 * [RISC-V - Debian Wiki](https://wiki.debian.org/RISC-V)

 * [RISC-V - Fedora Project Wiki](https://fedoraproject.org/wiki/Architectures/RISC-V)

 * [RISC-V - openSUSE Wiki](https://en.opensuse.org/openSUSE:RISC-V)
 
 * [RISC-V - Gentoo Linux Wiki](https://wiki.gentoo.org/wiki/RISC-V_Qemu_setup)]
 
 * [Alpine Linux riscv**64**](https://dl-cdn.alpinelinux.org/alpine/edge/releases/riscv64/)
 
 ### BSD-based Operating Systems
 [Back to the Top](#table-of-contents)
 
 * [RISC-V - FreeBSD Wiki](https://wiki.freebsd.org/riscv)

 * [RISC-V - OpenBSD Wiki](https://www.openbsd.org/riscv64.html)
 
 ### Real-Time Operating Systems (RTOS)
 [Back to the Top](#table-of-contents)
 
 * [FreeRTOS](https://freertos.org/) 

 * [Zephyr OS](https://www.zephyrproject.org/zephyr-rtos-featured-in-risc-v-getting-started-guide/) 

 * [meta-riscv AKA OpenEmbedded/Yocto](https://github.com/riscv/meta-riscv)

 * [Huawei LiteOS](https://www.huawei.com/minisite/liteos/en/index.html)

 * [Apache Mynewt](https://mynewt.apache.org/)

 * [Apache NuttX](https://nuttx.apache.org/)

 * [Drone OS](https://www.drone-os.com/)

 * [embOS](https://www.segger.com/products/rtos/embos/)

 * [Little Kernel Embedded Operating System](https://github.com/littlekernel/lk/)

 * [Tock OS](https://www.tockos.org/)

 * [TrampolineRTOS](https://github.com/TrampolineRTOS/trampoline)

 * [RIOT](https://www.riot-os.org/)  
 
 ### seL4 Operating Systems

[Back to the Top](#table-of-contents)

* **[seL4](https://sel4.systems/)** is a family of second-generation microkernels, used to implement a variety of operating systems.

[KataOS](https://github.com/AmbiML/sparrow-kata) is a a home-grown operating system that runs on top of [seL4](https://github.com/seL4) and is written almost entirely in [Rust](https://www.rust-lang.org/). It ignores the seL4 kernel using [Renode](https://antmicro.com/blog/2022/08/running-rust-programs-in-sel4/) simulator and related frameworks. KataOS is part of the [Sparrow](https://github.com/AmbiML/sparrow-manifest) project to build a low-power secure embeded platform for Ambient ML applications. The target platform leverages [RISC-V](https://riscv.org/) and [OpenTitan](https://opentitan.org/). 
 

## RISC-V Tools

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

[Rocket Chip Generator](https://github.com/chipsalliance/rocket-chip) is a repository contains the Rocket chip generator necessary to instantiate the RISC-V Rocket Core.

[CORE-V CVA6](https://github.com/openhwgroup/cva6) is an application class 6-stage RISC-V CPU capable of booting Linux.

[Cores-SweRV](https://github.com/chipsalliance/Cores-SweRV) is the EH1 RISC-V SweRV CoreTM 1.9 from Western Digital. 

[VRoom](https://github.com/MoonbaseOtago/vroom) is a new high-end RISC-V CPU implementation.

[FireSim](https://fires.im/) is an open-source cycle-accurate FPGA-accelerated full-system hardware simulation platform that runs on cloud FPGAs (Amazon EC2 F1).

[Nuclei Software Development Kit(Nuclei SDK)](https://doc.nucleisys.com/nuclei_sdk) is a toolkit for developing and evaluating software using our FPGA evaluation board.

[GAP SDK](https://github.com/GreenWaves-Technologies/gap_sdk) is set of tools and libraries that allows you to compile and execute applications on the GAP IoT Application Processor. This SDK provides a development environment for the GAP series processors.

[RISC-V Studio™ Integrated Development Environment (IDE)](https://riscv.studio) is a flexible and highly configurable software environment that helps the RISC-V developers discover, configure, develop, debug and deploy system designs utilizing open-source and commercial RISC-V IPs and platforms.

[Ashling RiscFree™ C/C++ for RISC-V](https://www.sifive.com/software) is a fully integrated development tool environment that includes an IDE, compiler, debugger, and Opella-XD JTAG probe ready to use with SiFive's RISC-V Core IP products. 

[RISCVEMU](https://riscv.org/software-tools/riscvemu/) is a system emulator developed by Fabrice Bellard for the RISC-V architecture. Its purpose is to be small and simple while being complete. Among its features are the support of 128 bit addressing and 128 bit floating point which makes the emulator ready for the future.

[RISC-V Interpreter](http://www.cs.cornell.edu/courses/cs3410/2019sp/riscv/interpreter/) is a online Interpreter for RISC-V build by Cornell University.

[Chipyard](https://chipyard.readthedocs.io/en/latest/) is an open source framework for agile development of Chisel-based systems-on-chip. It will allow you to leverage the Chisel HDL, Rocket Chip SoC generator, and other [Berkeley](https://berkeley.edu/) projects to produce a RISC-V SoC with everything from MMIO-mapped peripherals to custom accelerators.

[BRISC-V Explorer](https://ascslab.org/research/briscv/explorer/explorer.html) is a RISC-V CPU simulator application that runs in a browser allowing users to easily run it on Windows, Linux or Mac. In the BRISC-V Explorer, users can 

  - 1. Select their desired core type.
  - 2. Enter parameters such as memory size for that core.
  - 3. Configure cache parameters including block size and associativity.
  
 
[Ripes](https://github.com/mortbopet/Ripes) is a graphical processor simulator and assembly editor for the RISC-V instruction set architecture(ISA).

[OpenHW Group's RISC-V Virtual Machine (riscv_vm)](https://github.com/openhwgroup/riscv_vm/) is a set of instructions to import Ubuntu guest Virtual Machine for RISC-V development for the VEGA board. It's intended for anyone wanting to study, configure as-preferred, modify, implement or release hardware based the RISC-V Instruction Set Architecture. The VM is preconfigured for RISC-V HW development. 

[The Eclipse Embedded CDT](https://github.com/eclipse-embed-cdt/eclipse-plugins) is a collection of plug-ins for Arm & RISC-V C/C++ developers.

[PlatformIO](https://platformio.org/) is a professional collaborative platform for embedded development with no vendor lock-in. It provides support for multiplatforms and frameworks such as IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbed OS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V.

[PlatformIO for VSCode](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) is a plugin that provides support for the PlatformIO IDE on VSCode.

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

# FPGA Development

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/104069966-ab060f00-51ba-11eb-8295-d3479b485c86.png">
  <br />
</p>

## Models of FPGA Boards

[Checkout the PolarFire® FPGA Development Kits](https://www.microsemi.com/product-directory/dev-kits-solutions/3864-polarfire-kits)

<img src="https://user-images.githubusercontent.com/45159366/104068349-97a67400-51b9-11eb-82b5-d06f804400ee.png">


[Checkout the Artix 7 FPGA Development board](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)

<img src="https://user-images.githubusercontent.com/45159366/104068359-9d03be80-51b9-11eb-9bd2-0045e8f45eb9.png">


[Checkout the Spartan 6 FPGA Development board](https://store.digilentinc.com/anvyl-spartan-6-fpga-trainer-board/)

<img src="https://user-images.githubusercontent.com/45159366/104068361-9e34eb80-51b9-11eb-9c68-0b59c5a107e1.png">



[Checkout the Zynq-7000 for ARM/FPGA SoC Development board](https://store.digilentinc.com/cora-z7-zynq-7000-single-core-and-dual-core-options-for-arm-fpga-soc-development/)

<img src="https://user-images.githubusercontent.com/45159366/104068367-a12fdc00-51b9-11eb-966a-08a0868fcfb7.png">


## FPGA Learning Resources
 
[FPGA(Field Programmable Gate Arrays)](https://www.xilinx.com/products/silicon-devices/fpga/what-is-an-fpga.html) are semiconductor devices that are based around a matrix of configurable logic blocks (CLBs) connected via programmable interconnects. FPGAs can be reprogrammed to desired application or functionality requirements after manufacturing.

[TinyFPGA](https://tinyfpga.com) is a new series of boards that are low-cost, [open source FPGA boards](https://github.com/tinyfpga) in a tiny form factor.

[SiFive FPGA shells](https://github.com/sifive/fpga-shells)

[FPGA & SoC Design Tools from Microsemi](https://www.microsemi.com/product-directory/fpga-soc/1637-design-resources)

[QuickLogic Embedded FPGA (eFPGA) Intellectual Property (IP) and Software](https://www.quicklogic.com/products/efpga/efpga-ip-software/)

[FPGA for Beginners with Development Boards from Digilent®](https://store.digilentinc.com/fpga-for-beginners/)

[Hundreds of FPGA Projects on Instructables](https://www.instructables.com/circuits/howto/FPGA/)
 
[FPGA Fundamentals from NI(National Instruments)](https://www.ni.com/en-us/innovations/white-papers/08/fpga-fundamentals.html)

[Getting Started With LabVIEW FPGA from NI(National Instruments)](https://www.ni.com/tutorial/14532/en/)
 
[Programming and FPGA Basics - INTEL® FPGAS](https://www.intel.com/content/www/us/en/products/programmable/fpga/new-to-fpgas/resource-center/overview.html)
 
[Intel FPGA Training Program](https://www.intel.com/content/www/us/en/programmable/support/training/overview.html)
 
[FPGA Courses on Coursera](https://www.coursera.org/courses?query=fpga)
 
[FPGA Courses on Udemy](https://www.udemy.com/topic/fpga/)
 
[FPGA Online Training Courses on LinkedIn Learning](https://www.linkedin.com/learning/topics/fpga)

[UMass Lowell's Graduate Certificate in Field Programmable Gate Arrays(FPGA)](https://gps.uml.edu/certificates/grad/online-field-programmable-gate-arrays-bae-graduate-certificate.cfm)

[FPGA Design Fundamentals Course (UC San Diego Extension)](https://extension.ucsd.edu/courses-and-programs/fpga-design-fundamentals)

[FPGA II Course (UC San Diego Extension)](https://extension.ucsd.edu/courses-and-programs/fpga-embedded-design)

[FPGAs & SoCs Training from Microsemi](https://www.microsemi.com/product-directory/training/4244-fpgas-socs-training)
 
[DSP fundamentals for FPGAs course from MATLAB and Simulink Training](https://www.mathworks.com/training-schedule/dsp-for-fpgas.html)
 
[Verilog Courses on Coursera](https://www.coursera.org/courses?query=verilog)


## FPGA Tools

[LabVIEW FPGA](https://www.ni.com/en-us/shop/software/products/labview-fpga-module.html) is a software add-on for LabVIEW that you can use to more efficiently and effectively design FPGA-based systems through a highly integrated development environment, IP libraries, a high-fidelity simulator, and debugging features.

[Apio](https://github.com/FPGAwars/apio) is a multiplatform toolbox, with static pre-built packages, project configuration tools and easy command interface to verify, synthesize, simulate and upload your verilog designs.

[IceStorm](https://github.com/YosysHQ/icestorm) is a project that aims at documenting the bitstream format of Lattice iCE40 FPGAs and providing simple tools for analyzing and creating bitstream files.

[Icestudio](https://icestudio.io/) is a visual editor for open FPGA boards. Built on top of the Icestorm project using Apio.

[FuseSoC](https://github.com/olofk/fusesoc) is an award-winning package manager and a set of build tools for HDL (Hardware Description Language) code and FPGA/ASIC development.
 
[OpenWiFi](https://github.com/open-sdr/openwifi) is an open-source IEEE802.11/Wi-Fi baseband chip/FPGA design.
 
[PipeCNN](https://github.com/doonny/PipeCNN) is an OpenCL-based FPGA Accelerator for Large-Scale Convolutional Neural Networks (CNNs). Currently, there is a growing trend among developers in the FPGA community to utilize High Level Synthesis (HLS) tools to design and implement customized circuits on FPGAs.

[Verilator](https://verilator.org/) is an open-source SystemVerilog simulator and lint system.

[Verilog to Routing(VTR)](https://verilogtorouting.org/) is a collaborative project to provide a open-source framework for conducting FPGA architecture and CAD Research & Development. The VTR design flow takes as input a Verilog description of a digital circuit, and a description of the target FPGA architecture.

[PlatformIO](https://platformio.org/) is a professional collaborative platform for embedded development with no vendor lock-in. It provides support for multiplatforms and frameworks such as IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbed OS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V.

[PlatformIO for VSCode](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) is a plugin that provides support for the PlatformIO IDE on VSCode.
 
[Tock](https://www.tockos.org/) is an embedded operating system designed for running multiple concurrent, mutually distrustful applications on Cortex-M and RISC-V based embedded platforms. Tock's design centers around protection, both from potentially malicious applications and from device drivers. 

[OpenTimer](https://github.com/OpenTimer/OpenTimer) is a High-Performance Timing Analysis Tool for VLSI Systems.

[LLVM](https://github.com/llvm/) is a library that has collection of modular/reusable compiler and toolchain  components (assemblers, compilers, debuggers, etc.). With these components LLVM can be used as a compiler framework, providing a front-end(parser and lexer) and a back-end (code that converts LLVM's representation to actual machine code).

[TinyGo](https://tinygo.org/) is a Go compiler(based on LLVM) intended for use in small places such as microcontrollers, WebAssembly (Wasm), and command-line tools.

[Chipyard](https://chipyard.readthedocs.io/en/latest/) is an open source framework for agile development of Chisel-based systems-on-chip. It will allow you to leverage the Chisel HDL, Rocket Chip SoC generator, and other [Berkeley](https://berkeley.edu/) projects to produce a RISC-V SoC with everything from MMIO-mapped peripherals to custom accelerators.

[The Eclipse Embedded CDT](https://github.com/eclipse-embed-cdt/eclipse-plugins) is a collection of plug-ins for Arm & RISC-V C/C++ developers.
[Unicorn](https://github.com/unicorn-engine/unicorn) is a lightweight, multi-platform, multi-architecture CPU emulator framework(ARM, AArch64, M68K, Mips, Sparc, X86) based on [QEMU](https://www.qemu.org/).

[Keystone](https://github.com/keystone-engine/keystone) is a lightweight multi-platform, multi-architecture(Arm, Arm64, Hexagon, Mips, PowerPC, Sparc, SystemZ & X86) assembler framework.

[Reko](https://github.com/uxmal/reko) is a decompiler for machine code binaries.

[Renode](https://renode.io/) is [Antmicro's](https://antmicro.com) virtual development framework for multinode embedded networks (both wired and wireless) and is intended to enable a scalable workflow for creating effective, tested and secure IoT systems.

[Diosix](https://diosix.org/) is a lightweight, secure, multiprocessor bare-metal hypervisor written in Rust for RISC-V.

# Verilog/SystemVerilog Development

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/102273517-4b785480-3ed7-11eb-910a-113821428f17.png">
  <br />

</p>

## Verilog/SystemVerilog Learning Resources

[Verilog](https://verilog.com/) is a Hardware Description Language(HDL) used to design and document electronic systems. Verilog HDL allows designers to design at various levels of abstraction.

[SystemVerilog](https://www.systemverilog.io/) is an extension of Verilog with many of the verification features that allow engineers to verifythe design using complex testbench structures and random stimuli in simulation. 

[Verilog Book Shelf](https://verilog.com/v-books.html)

[Verilog HDL Basics training from Intel](https://www.intel.com/content/www/us/en/programmable/support/training/course/ohdl1120.html)

[SystemVerilog for Design and Verification](https://www.cadence.com/en_US/home/training/all-courses/82143.html)

[Verilog HDL Programming Courses on Udemy](https://www.udemy.com/topic/verilog-hdl-programming/)

[Top Verilog Programming Courses on Coursera](https://www.coursera.org/courses?query=verilog)

[Verilog course for Engineers on Technobyte](https://technobyte.org/verilog-course-tutorials/)

[Verilog Tutorials and Courses on hackr.io](https://hackr.io/tutorials/learn-verilog)

[Designing With Verilog Certification from the Xilinx Learning Center](https://xilinxprod-catalog.netexam.com/Certification/35916/designing-with-verilog)

[Learning Verilog for FPGA Development on LinkedIn Learning](https://www.linkedin.com/learning/learning-verilog-for-fpga-development)

[SystemVerilog tutorial on ChipVerify](https://www.chipverify.com/systemverilog/systemverilog-tutorial)

## Verilog/SystemVerilog Tools

[Apio](https://github.com/FPGAwars/apio) is a multiplatform toolbox, with static pre-built packages, project configuration tools and easy command interface to verify, synthesize, simulate and upload your verilog designs.

[IceStorm](https://github.com/YosysHQ/icestorm) is a project that aims at documenting the bitstream format of Lattice iCE40 FPGAs and providing simple tools for analyzing and creating bitstream files.

[Icestudio](https://icestudio.io/) is a visual editor for open FPGA boards. Built on top of the Icestorm project using Apio.

[EDA Playground](https://www.edaplayground.com) is a online code for programming your Verilog projects.

[PlatformIO](https://platformio.org/) is a professional collaborative platform for embedded development with no vendor lock-in. It provides support for multiplatforms and frameworks such as IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbed OS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V.

[PlatformIO for VSCode](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) is a plugin that provides support for the PlatformIO IDE on VSCode.

[Chisel](https://www.chisel-lang.org/) is a hardware design language that facilitates advanced circuit generation and design reuse for both ASIC and FPGA digital logic designs. Chisel adds hardware construction primitives to the [Scala](https://www.scala-lang.org/) programming language, providing designers with the power of a modern programming language to write complex, parameterizable circuit generators that produce synthesizable Verilog.

[Clash compiler](https://www.clash-lang.org/) is a functional hardware description language that borrows both its syntax and semantics from the functional programming language Haskell. The Clash compiler transforms these high-level descriptions to low-level synthesizable VHDL, Verilog, or SystemVerilog.

[Verilator](https://verilator.org/) is an open-source SystemVerilog simulator and lint system.

[Verilog to Routing(VTR)](https://verilogtorouting.org/) is a collaborative project to provide a open-source framework for conducting FPGA architecture and CAD Research & Development. The VTR design flow takes as input a Verilog description of a digital circuit, and a description of the target FPGA architecture.

[Cascade](https://github.com/vmware/cascade) is a Just-In-Time Compiler for Verilog from VMware Research. Cascade executes code immediately in a software simulator, and performs compilation in the background. When compilation is finished, the code is moved into hardware, and from the user’s perspective it simply gets faster over time.

[OpenTimer](https://github.com/OpenTimer/OpenTimer) is a High-Performance Timing Analysis Tool for VLSI Systems.

# Assembly Development
[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/101415607-18154480-389d-11eb-80e8-17a5c57e480f.png">
  <br />
</p>

**[Learn Risc-V Assembly Programming](https://riscv.org/news/2021/01/learn-risc-v-assembly-programming-lesson1-for-absolute-beginners-chibiakumas/)**

## Assembly Learning Resources

[Assembly](https://en.wikipedia.org/wiki/Assembly_language) is a low-level programming language. It uses mnemonic codes and labels to represent machine-level code with each instruction corresponding to just one machine operation.

[RISC-V Foundation](https://riscv.org/) is a non-profit corporation controlled by its 500 members(NVIDIA, Google, Samsung, Raspberry Pi, SiFive, Canonical, and Western Digital) to drive forward the adoption and implementation of the free and open RISC-V instruction set architecture (ISA).

[Intel® 64 and IA-32 Architectures Software Developer’s Manual](https://software.intel.com/content/www/us/en/develop/articles/intel-sdm.html)

[Introduction to x64 Assembly from Intel](https://software.intel.com/content/www/us/en/develop/articles/introduction-to-x64-assembly.html)

[x86 Assembly Language Reference Manual for Open Solaris](https://docs.oracle.com/cd/E19120-01/open.solaris/817-5477/index.html)

[AMD64 Architecture Programmer’s Manual Volume 1-5](https://www.amd.com/system/files/TechDocs/40332.pdf)

[AMD GPU ISA documentation](https://gpuopen.com/documentation/amd-isa-documentation/)

[AMD Developer Guides, Manuals, and ISA Documents](https://developer.amd.com/resources/developer-guides-manuals/)

[Assembler language from IBM](https://www.ibm.com/support/knowledgecenter/en/SSLTBW_2.1.0/com.ibm.zos.v2r1.asma400/asmr102112.htm)

[The Assembler language on z/OS from IBM](https://www.ibm.com/support/knowledgecenter/zosbasics/com.ibm.zos.zappldev/zappldev_25.htm)

[MIPS Architecture & Technology from Wave Computing](https://wavecomp.ai/mips-technology/)

[Assemblies in .NET](https://docs.microsoft.com/en-us/dotnet/standard/assembly/)

[Microsoft Macro Assembler reference](https://docs.microsoft.com/en-us/cpp/assembler/masm/microsoft-macro-assembler-reference)

[Compiler Intrinsics and Assembly Language from Microsoft](https://docs.microsoft.com/en-us/cpp/intrinsics/compiler-intrinsics-and-assembly-language)

[x86 and amd64 instruction Reference](https://www.felixcloutier.com/x86/)

[Intro to x86 Assembly Language Programming](https://cs.lmu.edu/~ray/notes/x86assembly/)

[Learn Assembly Programming courses on Udemy](https://www.udemy.com/topic/assembly-language/)

[Assembly Languages and Assemblers courses on Coursera](https://www.coursera.org/lecture/build-a-computer/unit-6-1-assembly-languages-and-assemblers-l4EGm)

[Intro to Assembly Language from MIT](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-004-computation-structures-spring-2017/index.htm)

## Assembly Tools & Architectures

[Arm Instruction Emulator (ArmIE)](https://developer.arm.com/tools-and-software/server-and-hpc/compile/arm-instruction-emulator/resources/tutorials) is a tool that emulates Scalable Vector Extension (SVE) and SVE2 instructions on AArch64/ARM64 platforms. 

[FASM (flat assembler)](https://flatassembler.net/) is an assembler for x86 processors that supports Intel-based assembly language on the IA-32 and x86-64 computer architectures. 

[Microsoft Assembler (MASM) for x64](https://docs.microsoft.com/en-us/cpp/assembler/masm/masm-for-x64-ml64-exe) is Microsoft's assembler that accepts x64 assembler language. 

[MASM/TASM](https://github.com/xsro/masm-tasm) is a VSCode extension that offers a way to run and debug DOS(80x86) assembly TASM/MASM through DOSBox and msdos-player.

[NASM](https://nasm.us/) is an asssembler/disassembler for the x86 CPU architecture portable to nearly every modern platform, and with code generation for many platforms old and new.

[GAS](https://www.gnu.org/software/binutils/) is the assembler used by the GNU Project for the default back-end of GCC. It is used to assemble the GNU operating system and the Linux kernel.

[MIPS](https://en.wikipedia.org/wiki/MIPS_Technologies) is a reduced instruction set computer (RISC) instruction set architecture (ISA) developed by [MIPS Technologies, Inc.](https://www.mips.com/). In June 2018 [MIPS was Acquired by AI Startup Wave Computing](https://www.top500.org/news/mips-acquired-by-ai-startup-wave-computing/).

[LLVM](https://github.com/llvm/) is a library that has collection of modular/reusable compiler and toolchain  components (assemblers, compilers, debuggers, etc.). With these components LLVM can be used as a compiler framework, providing a front-end(parser and lexer) and a back-end (code that converts LLVM's representation to actual machine code).

[TinyGo](https://tinygo.org/) is a Go compiler(based on LLVM) intended for use in small places such as microcontrollers, WebAssembly (Wasm), and command-line tools.

[Tock](https://www.tockos.org/) is an embedded operating system designed for running multiple concurrent, mutually distrustful applications on Cortex-M and RISC-V based embedded platforms. Tock's design centers around protection, both from potentially malicious applications and from device drivers. 

[PlatformIO](https://platformio.org/) is a professional collaborative platform for embedded development with no vendor lock-in. It provides support for multiplatforms and frameworks such as IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbed OS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V.

[PlatformIO for VSCode](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) is a plugin that provides support for the PlatformIO IDE on VSCode.

[Keystone](https://github.com/keystone-engine/keystone) is a lightweight multi-platform, multi-architecture(Arm, Arm64, Hexagon, Mips, PowerPC, Sparc, SystemZ & X86) assembler framework.

[Unicorn](https://github.com/unicorn-engine/unicorn) is a lightweight, multi-platform, multi-architecture CPU emulator framework(ARM, AArch64, M68K, Mips, Sparc, X86) based on [QEMU](https://www.qemu.org/).

# Telco 5G Development
[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

 <img src="https://user-images.githubusercontent.com/45159366/105409952-14881380-5be6-11eb-84fc-b07db69698ed.png">

 **VMware Cloud First Approach. Source: [VMware](https://www.vmware.com/products/telco-cloud-automation.html).**


 <img src="https://user-images.githubusercontent.com/45159366/105409956-1520aa00-5be6-11eb-8215-735c92a5470c.png">

 **VMware Telco Cloud Automation Components. Source: [VMware](https://www.vmware.com/products/telco-cloud-automation.html).**


## Telco 5G Learning Resources

[HPE(Hewlett Packard Enterprise) Telco Blueprints overview](https://techhub.hpe.com/eginfolib/servers/docs/Telco/Blueprints/infocenter/index.html#GUID-9906A227-C1FB-4FD5-A3C3-F3B72EC81CAB.html)

[Network Functions Virtualization Infrastructure (NFVI) by Cisco](https://www.cisco.com/c/en/us/solutions/service-provider/network-functions-virtualization-nfv-infrastructure/index.html)

[Introduction to vCloud NFV Telco Edge from VMware](https://docs.vmware.com/en/VMware-vCloud-NFV-OpenStack-Edition/3.1/vloud-nfv-edge-reference-arch-31/GUID-744C45F1-A8D5-4523-9E5E-EAF6336EE3A0.html)

[VMware Telco Cloud Automation(TCA) Architecture Overview](https://docs.vmware.com/en/VMware-Telco-Cloud-Platform-5G-Edition/1.0/telco-cloud-platform-5G-edition-reference-architecture/GUID-C19566B3-F42D-4351-BA55-DE70D55FB0DD.html)

[5G Telco Cloud from VMware](https://telco.vmware.com/)

[Maturing OpenStack Together To Solve Telco Needs from Red Hat](https://www.redhat.com/cms/managed-files/4.Nokia%20CloudBand%20&%20Red%20Hat%20-%20Maturing%20Openstack%20together%20to%20solve%20Telco%20needs%20Ehud%20Malik,%20Senior%20PLM,%20Nokia%20CloudBand.pdf)

[Red Hat telco ecosystem program](https://connect.redhat.com/en/programs/telco-ecosystem)

[OpenStack for Telcos by Canonical](https://ubuntu.com/blog/openstack-for-telcos-by-canonical)

[Open source NFV platform for 5G from Ubuntu](https://ubuntu.com/telco)

[Understanding 5G Technology from Verizon](https://www.verizon.com/5g/)

[Verizon and Unity partner to enable 5G & MEC gaming and enterprise applications](https://www.verizon.com/about/news/verizon-unity-partner-5g-mec-gaming-enterprise)

[Understanding 5G Technology from Intel](https://www.intel.com/content/www/us/en/wireless-network/what-is-5g.html)

[Understanding 5G Technology from Qualcomm](https://www.qualcomm.com/invention/5g/what-is-5g)

[Telco Acceleration with Xilinx](https://www.xilinx.com/applications/wired-wireless/telco.html)

[VIMs on OSM Public Wiki](https://osm.etsi.org/wikipub/index.php/VIMs)

[Amazon EC2 Overview and Networking Introduction for Telecom Companies](https://docs.aws.amazon.com/whitepapers/latest/ec2-networking-for-telecom/ec2-networking-for-telecom.pdf)

[Citrix Certified Associate – Networking(CCA-N)](http://training.citrix.com/cms/index.php/certification/networking/)

[Citrix Certified Professional – Virtualization(CCP-V)](https://www.globalknowledge.com/us-en/training/certification-prep/brands/citrix/section/virtualization/citrix-certified-professional-virtualization-ccp-v/)

[CCNP Routing and Switching](https://learningnetwork.cisco.com/s/ccnp-enterprise)

[Certified Information Security Manager(CISM)](https://www.isaca.org/credentialing/cism)

[Wireshark Certified Network Analyst (WCNA)](https://www.wiresharktraining.com/certification.html)

[Juniper Networks Certification Program Enterprise (JNCP)](https://www.juniper.net/us/en/training/certification/)

[Cloud Native Computing Foundation Training and Certification Program](https://www.cncf.io/certification/training/)


## Telco 5G Tools and Frameworks

[Open Stack](https://www.openstack.org/) is an open source cloud platform, deployed as infrastructure-as-a-service (IaaS) to orchestrate data center operations on bare metal, private cloud hardware, public cloud resources, or both (hybrid/multi-cloud architecture). OpenStack includes advance use of virtualization & SDN for network traffic optimization to handle the core cloud-computing services of compute, networking, storage, identity, and image services.

[StarlingX](https://www.starlingx.io/) is a complete cloud infrastructure software stack for the edge used by the most demanding applications in industrial IOT, telecom, video delivery and other ultra-low latency use cases.

[Airship](https://www.airshipit.org/) is a collection of open source tools for automating cloud provisioning and management. Airship provides a declarative framework for defining and managing the life cycle of open infrastructure tools and the underlying hardware.

[Network functions virtualization (NFV)](https://www.vmware.com/topics/glossary/content/network-functions-virtualization-nfv) is the replacement of network appliance hardware with virtual machines. The virtual machines use a hypervisor to run networking software and processes such as routing and load balancing. NFV allows for the separation of communication services from dedicated hardware, such as routers and firewalls. This separation means network operations can provide new services dynamically and without installing new hardware. Deploying network components with network functions virtualization only takes hours compared to months like with traditional networking solutions.

[Software Defined Networking (SDN)](https://www.vmware.com/topics/glossary/content/software-defined-networking) is an approach to networking that uses software-based controllers or application programming interfaces (APIs) to communicate with underlying hardware infrastructure and direct traffic on a network. This model differs from that of traditional networks, which use dedicated hardware devices (routers and switches) to control network traffic.

[Virtualized Infrastructure Manager (VIM)](https://www.cisco.com/c/en/us/td/docs/net_mgmt/network_function_virtualization_Infrastructure/3_2_2/install_guide/Cisco_VIM_Install_Guide_3_2_2/Cisco_VIM_Install_Guide_3_2_2_chapter_00.html) is a service delivery and reduce costs with high performance lifecycle management Manage the full lifecycle of the software and hardware comprising your NFV infrastructure (NFVI), and maintaining a live inventory and allocation plan of both physical and virtual resources.

[Management and Orchestration(MANO)](https://www.etsi.org/technologies/open-source-mano) is an ETSI-hosted initiative to develop an Open Source NFV Management and Orchestration (MANO) software stack aligned with ETSI NFV. Two of the key components of the ETSI NFV architectural framework are the NFV Orchestrator and VNF Manager, known as NFV MANO.

[Magma](https://www.magmacore.org/) is an open source software platform that gives network operators an open, flexible and extendable mobile core network solution. Their mission is to connect the world to a faster network by enabling service providers to build cost-effective and extensible carrier-grade networks. Magma is 3GPP generation (2G, 3G, 4G or upcoming 5G networks) and access network agnostic (cellular or WiFi). It can flexibly support a radio access network with minimal development and deployment effort.

[OpenRAN](https://open-ran.org/) is an intelligent Radio Access Network(RAN) integrated on general purpose platforms with open interface between software defined functions. Open RANecosystem enables enormous flexibility and interoperability with a complete openess to multi-vendor deployments.

[Open vSwitch(OVS)](https://www.openvswitch.org/)is an open source production quality, multilayer virtual switch licensed under the open source Apache 2.0 license. It is designed to enable massive network automation through programmatic extension, while still supporting standard management interfaces and protocols (NetFlow, sFlow, IPFIX, RSPAN, CLI, LACP, 802.1ag).

[Edge](https://www.ibm.com/cloud/what-is-edge-computing) is a distributed computing framework that brings enterprise applications closer to data sources such as IoT devices or local edge servers. This proximity to data at its source can deliver strong business benefits, including faster insights, improved response times and better bandwidth availability.

[Multi-access edge computing (MEC)](https://www.etsi.org/technologies/multi-access-edge-computing) is an Industry Specification Group (ISG) within ETSI to create a standardized, open environment which will allow the efficient and seamless integration of applications from vendors, service providers, and third-parties across multi-vendor Multi-access Edge Computing platforms.

[Virtualized network functions(VNFs)](https://www.juniper.net/documentation/en_US/cso4.1/topics/concept/nsd-vnf-overview.html) is a software application used in a Network Functions Virtualization (NFV) implementation that has well defined interfaces, and provides one or more component networking functions in a defined way. For example, a security VNF provides Network Address Translation (NAT) and firewall component functions.

[Cloud-Native Network Functions(CNF)](https://www.cncf.io/announcements/2020/11/18/cloud-native-network-functions-conformance-launched-by-cncf/) is a network function designed and implemented to run inside containers. CNFs inherit all the cloud native architectural and operational principles including Kubernetes(K8s) lifecycle management, agility, resilience, and observability.

[Physical Network Function(PNF)](https://www.mpirical.com/glossary/pnf-physical-network-function) is a physical network node which has not undergone virtualization. Both PNFs and VNFs (Virtualized Network Functions) can be used to form an overall Network Service.

[Network functions virtualization infrastructure(NFVI)](https://docs.vmware.com/en/VMware-vCloud-NFV/2.0/vmware-vcloud-nfv-reference-architecture-20/GUID-FBEA6C6B-54D8-4A37-87B1-D825F9E0DBC7.html) is the foundation of the overall NFV architecture. It provides the physical compute, storage, and networking hardware that hosts the VNFs. Each NFVI block can be thought of as an NFVI node and many nodes can be deployed and controlled geographically.

## Containers

[Open Container Initiative](https://opencontainers.org/about/overview/) is an open governance structure for the express purpose of creating open industry standards around container formats and runtimes.

[Kubernetes](https://kubernetes.io/) is an open-source container-orchestration system for automating application deployment, scaling, and management. It was originally designed by Google, and is now maintained by the Cloud Native Computing Foundation.

[Google Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine/) is a managed, production-ready environment for deploying containerized applications.

[OpenShift](https://www.openshift.com/) is focused on security at every level of the container stack and throughout the application lifecycle. It includes long-term, enterprise support from one of the leading Kubernetes contributors and open source software companies.

[Rancher](https://rancher.com/) is a complete software stack for teams adopting containers. It addresses the operational and security challenges of managing multiple Kubernetes clusters, while providing DevOps teams with integrated tools for running containerized workloads.

[Docker](https://www.docker.com/) is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels. All containers are run by a single operating-system kernel and are thus more lightweight than virtual machines.

[Dockle](https://containers.goodwith.tech/) is a Container Image Linter for Security, Helping build the Best-Practice Docker Image.

[TwistLock](https://www.esecurityplanet.com/products/twistlock/) is a Cloud Native Cybersecurity Platform that provides full lifecycle security for containerized environments. From pipeline to perimeter, Twistlock helps customers scale securely and deploy containers with confidence. The Twistlock Platform goes beyond just containers to secure the entire cloud native stack, from the host OS to serverless functions.

[Rook](https://rook.io/) is an open source cloud-native storage orchestrator for Kubernetes that turns distributed storage systems into self-managing, self-scaling, self-healing storage services. It automates the tasks of a storage administrator: deployment, bootstrapping, configuration, provisioning, scaling, upgrading, migration, disaster recovery, monitoring, and resource management.

[Rkt](https://coreos.com/rkt/) is a pod-native container engine for Linux. It is composable, secure, and built on standards.

[OpenEBS](https://openebs.io/) is a Kubernetes-based tool to create stateful applications using Container Attached Storage.

[Container Storage Interface (CSI)](https://www.architecting.it/blog/container-storage-interface/). CSI is an API that lets container orchestration platforms like Kubernetes seamlessly communicate with stored data via a plug-in.

[Open Container Initiative](https://opencontainers.org/about/overview/) is an open governance structure for the express purpose of creating open industry standards around container formats and runtimes.

[Buildah](https://buildah.io/) is a command line tool to build Open Container Initiative (OCI) images. It can be used with Docker, Podman, Kubernetes.

[Podman](https://podman.io/) is a daemonless, open source, Linux native tool designed to make it easy to find, run, build, share and deploy applications using Open Containers Initiative (OCI) Containers and Container Images. Podman provides a command line interface (CLI) familiar to anyone who has used the Docker Container Engine.

[Containerd](https://containerd.io) is a daemon that manages the complete container lifecycle of its host system, from image transfer and storage to container execution and supervision to low-level storage to network attachments and beyond. It is available for Linux and Windows.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/113521413-2ffc8c80-954e-11eb-9d19-b9c996bc524b.png">
  <br />
</p>

**Container Architecture. Source: [Containerd.io](https://containerd.io)**
 
# Kubernetes

[Back to the Top](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#table-of-contents)

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/95383873-a884d800-08a0-11eb-8eaf-57af5b119f56.png">
</p>

[Kubernetes (K8s)](https://kubernetes.io/) is an open-source system for automating deployment, scaling, and management of containerized applications. 

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/105645195-db9ea780-5e4e-11eb-8357-fb38b2f06d74.png">

**Building Highly-Availability(HA) Clusters with kubeadm. Source: [Kubernetes.io](https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/high-availability/), 2020**
</p>

[Google Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine/) is a managed, production-ready environment for running containerized applications.

[Azure Kubernetes Service (AKS)](https://azure.microsoft.com/en-us/services/kubernetes-service/) is serverless Kubernetes, with a integrated continuous integration and continuous delivery (CI/CD) experience, and enterprise-grade security and governance. Unite your development and operations teams on a single platform to rapidly build, deliver, and scale applications with confidence.

[Amazon EKS](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html) is a tool that runs Kubernetes control plane instances across multiple Availability Zones to ensure high availability.

[AWS Controllers for Kubernetes (ACK)](https://aws.amazon.com/blogs/containers/aws-controllers-for-kubernetes-ack/) is a new tool that lets you directly manage AWS services from Kubernetes. ACK makes it simple to build scalable and highly-available Kubernetes applications that utilize AWS services.

[Container Engine for Kubernetes (OKE)](https://www.oracle.com/cloud-native/container-engine-kubernetes/) is an Oracle-managed container orchestration service that can reduce the time and cost to build modern cloud native applications. Unlike most other vendors, Oracle Cloud Infrastructure provides Container Engine for Kubernetes as a free service that runs on higher-performance, lower-cost compute.

[Anthos](https://cloud.google.com/anthos/docs/concepts/overview) is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments.

[Red Hat Openshift](https://www.openshift.com/) is a fully managed Kubernetes platform that provides a foundation for on-premises, hybrid, and multicloud deployments. 

[OKD](https://okd.io/) is a community distribution of Kubernetes optimized for continuous application development and multi-tenant deployment. OKD adds developer and operations-centric tools on top of Kubernetes to enable rapid application development, easy deployment and scaling, and long-term lifecycle maintenance for small and large teams.

[Odo](https://odo.dev/) is a fast, iterative, and straightforward CLI tool for developers who write, build, and deploy applications on Kubernetes and OpenShift.

[Kata Operator](https://github.com/openshift/kata-operator) is an operator to perform lifecycle management (install/upgrade/uninstall) of [Kata Runtime](https://katacontainers.io/) on Openshift as well as Kubernetes cluster.

[Thanos](https://thanos.io/) is a set of components that can be composed into a highly available metric system with unlimited storage capacity, which can be added seamlessly on top of existing Prometheus deployments.

[OpenShift Hive](https://github.com/openshift/hive) is an operator which runs as a service on top of Kubernetes/OpenShift. The Hive service can be used to provision and perform initial configuration of OpenShift 4 clusters.

[Rook](https://rook.io/) is a tool that turns distributed storage systems into self-managing, self-scaling, self-healing storage services. It automates the tasks of a storage administrator: deployment, bootstrapping, configuration, provisioning, scaling, upgrading, migration, disaster recovery, monitoring, and resource management.

[VMware Tanzu](https://tanzu.vmware.com/tanzu) is a centralized management platform for consistently operating and securing your Kubernetes infrastructure and modern applications across multiple teams and private/public clouds.

[Kubespray](https://kubespray.io/) is a tool that combines Kubernetes and Ansible to easily install Kubernetes clusters that can be deployed on [AWS](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/aws.md), GCE, [Azure](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/azure.md), [OpenStack](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/openstack.md), [vSphere](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/vsphere.md), [Packet](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/packet.md) (bare metal), Oracle Cloud Infrastructure (Experimental), or Baremetal.

[KubeInit](https://github.com/kubeinit/kubeinit) provides Ansible playbooks and roles for the deployment and configuration of multiple Kubernetes distributions.

[Rancher](https://rancher.com/) is a complete software stack for teams adopting containers. It addresses the operational and security challenges of managing multiple Kubernetes clusters, while providing DevOps teams with integrated tools for running containerized workloads.

[K3s](https://github.com/rancher/k3s) is a highly available, certified Kubernetes distribution designed for production workloads in unattended, resource-constrained, remote locations or inside IoT appliances. 

[Helm](https://helm.sh/) is a Kubernetes Package Manager tool that makes it easier to install and manage Kubernetes applications.

[Knative](https://knative.dev/) is a Kubernetes-based platform to build, deploy, and manage modern serverless workloads. Knative takes care of the operational overhead details of networking, autoscaling (even to zero), and revision tracking. 

[KubeFlow](https://www.kubeflow.org/) is a tool dedicated to making deployments of machine learning (ML) workflows on Kubernetes simple, portable and scalable.

[Etcd](https://etcd.io/) is a distributed key-value store that provides a reliable way to store data that needs to be accessed by a distributed system or cluster of machines. Etcd is used as the backend for service discovery and stores cluster state and configuration for Kubernetes.

[OpenEBS](https://openebs.io/) is a Kubernetes-based tool to create stateful applications using Container Attached Storage.

[Container Storage Interface (CSI)](https://www.architecting.it/blog/container-storage-interface/) is an API that lets container orchestration platforms like Kubernetes seamlessly communicate with stored data via a plug-in.

[MicroK8s](https://microk8s.io/) is a tool that delivers the full Kubernetes experience. In a Fully containerized deployment with compressed over-the-air updates for ultra-reliable operations. It is supported on Linux, Windows, and MacOS.

[Charmed Kubernetes](https://ubuntu.com/kubernetes/features) is a well integrated, turn-key, conformant Kubernetes platform, optimized for your multi-cloud environments developed by Canonical.

[Grafana Kubernetes App](https://grafana.com/grafana/plugins/grafana-kubernetes-app) is a toll that allows you to monitor your Kubernetes cluster's performance. It includes 4 dashboards, Cluster, Node, Pod/Container and Deployment. It allows for the automatic deployment of the required Prometheus exporters and a default scrape config to use with your in cluster Prometheus deployment.

[KubeEdge](https://kubeedge.io/en/) is an open source system for extending native containerized application orchestration capabilities to hosts at Edge.It is built upon kubernetes and provides fundamental infrastructure support for network, app. deployment and metadata synchronization between cloud and edge.

[Lens](https://k8slens.dev/)  is the most powerful IDE for people who need to deal with Kubernetes clusters on a daily basis. It has support for MacOS, Windows and Linux operating systems.

[kind](https://kind.sigs.k8s.io/) is a tool for running local Kubernetes clusters using Docker container “nodes”. It was primarily designed for testing Kubernetes itself, but may be used for local development or CI.

[Flux CD](https://fluxcd.io/) is a tool that automatically ensures that the state of your Kubernetes cluster matches the configuration you've supplied in Git. It uses an operator in the cluster to trigger deployments inside Kubernetes, which means that you don't need a separate continuous delivery tool.

## Kubernetes Learning Resources

[Getting Kubernetes Certifications](https://training.linuxfoundation.org/certification/catalog/?_sft_technology=kubernetes)

[Getting started with Kubernetes on AWS](https://aws.amazon.com/kubernetes/)

[Kubernetes on Microsoft Azure](https://azure.microsoft.com/en-us/topic/what-is-kubernetes/)

[Intro to Azure Kubernetes Service](https://docs.microsoft.com/en-us/azure/aks/kubernetes-dashboard)

[Getting started with Google Cloud](https://cloud.google.com/learn/what-is-kubernetes)

[Getting started with Kubernetes on Red Hat](https://www.redhat.com/en/topics/containers/what-is-kubernetes)

[Getting started with Kubernetes on IBM](https://www.ibm.com/cloud/learn/kubernetes)

[YAML basics in Kubernetes](https://developer.ibm.com/technologies/containers/tutorials/yaml-basics-and-usage-in-kubernetes/)

[Elastic Cloud on Kubernetes](https://www.elastic.co/elastic-cloud-kubernetes)

[Docker and Kubernetes](https://www.docker.com/products/kubernetes)

[Deploy a model to an Azure Kubernetes Service cluster](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-deploy-azure-kubernetes-service?tabs=python)

[Simplify Machine Learning Inference on Kubernetes with Amazon SageMaker Operators](https://aws.amazon.com/blogs/machine-learning/simplify-machine-learning-inference-on-kubernetes-with-amazon-sagemaker-operators/)

[Running Apache Spark on Kubernetes](http://spark.apache.org/docs/latest/running-on-kubernetes.html)

[Kubernetes Across VMware vRealize Automation](https://blogs.vmware.com/management/2019/06/kubernetes-across-vmware-cloud-automation-services.html)

[VMware Tanzu Kubernetes Grid](https://tanzu.vmware.com/kubernetes-grid)

[All the Ways VMware Tanzu Works with AWS](https://tanzu.vmware.com/content/blog/all-the-ways-vmware-tanzutm-works-with-aws)

[VMware Tanzu Education](https://tanzu.vmware.com/education)

[Using Ansible in a Cloud-Native Kubernetes Environment](https://www.ansible.com/blog/how-useful-is-ansible-in-a-cloud-native-kubernetes-environment)

[Managing Kubernetes (K8s) objects with Ansible](https://docs.ansible.com/ansible/latest/collections/community/kubernetes/k8s_module.html)

[Setting up a Kubernetes cluster using Vagrant and Ansible](https://kubernetes.io/blog/2019/03/15/kubernetes-setup-using-ansible-and-vagrant/)

[Running MongoDB with Kubernetes](https://www.mongodb.com/kubernetes)

[Kubernetes Fluentd](https://docs.fluentd.org/v/0.12/articles/kubernetes-fluentd)

[Understanding the new GitLab Kubernetes Agent](https://about.gitlab.com/blog/2020/09/22/introducing-the-gitlab-kubernetes-agent/)

[Kubernetes Contributors](https://www.kubernetes.dev/)

[KubeAcademy from VMware](https://kube.academy/)

# Machine Learning

[Back to the Top](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/108111395-756e0480-7049-11eb-85ca-b87315e9d3ef.jpeg">
 </p>

 
 ## ML frameworks & applications

[TensorFlow Lite](https://www.tensorflow.org/lite/guide) is a set of tools to help developers run TensorFlow models on mobile, embedded, and IoT devices. It enables on-device machine learning inference with low latency and a small binary size.

[PyTorch](https://pytorch.org) is a library for deep learning on irregular input data such as graphs, point clouds, and manifolds. Primarily developed by Facebook's AI Research lab.

[Amazon SageMaker](https://aws.amazon.com/sagemaker/) is a fully managed service that provides every developer and data scientist with the ability to build, train, and deploy machine learning (ML) models quickly. SageMaker removes the heavy lifting from each step of the machine learning process to make it easier to develop high quality models.

[Azure Databricks](https://azure.microsoft.com/en-us/services/databricks/) is a fast and collaborative Apache Spark-based big data analytics service designed for data science and data engineering. Azure Databricks, sets up your Apache Spark environment in minutes, autoscale, and collaborate on shared projects in an interactive workspace. Azure Databricks supports Python, Scala, R, Java, and SQL, as well as data science frameworks and libraries including TensorFlow, PyTorch, and scikit-learn.

[Microsoft Cognitive Toolkit (CNTK)](https://docs.microsoft.com/en-us/cognitive-toolkit/) is an open-source toolkit for commercial-grade distributed deep learning. It describes neural networks as a series of computational steps via a directed graph. CNTK allows the user to easily realize and combine popular model types such as feed-forward DNNs, convolutional neural networks (CNNs) and recurrent neural networks (RNNs/LSTMs). CNTK implements stochastic gradient descent (SGD, error backpropagation) learning with automatic differentiation and parallelization across multiple GPUs and servers.

[Apache Airflow](https://airflow.apache.org) is an open-source workflow management platform created by the community to programmatically author, schedule and monitor workflows. Install. Principles. Scalable. Airflow has a modular architecture and uses a message queue to orchestrate an arbitrary number of workers. Airflow is ready to scale to infinity.

[Open Neural Network Exchange(ONNX)](https://github.com/onnx) is an open ecosystem that empowers AI developers to choose the right tools as their project evolves. ONNX provides an open source format for AI models, both deep learning and traditional ML. It defines an extensible computation graph model, as well as definitions of built-in operators and standard data types.

[Apache MXNet](https://mxnet.apache.org/) is a deep learning framework designed for both efficiency and flexibility. It allows you to mix symbolic and imperative programming to maximize efficiency and productivity. At its core, MXNet contains a dynamic dependency scheduler that automatically parallelizes both symbolic and imperative operations on the fly. A graph optimization layer on top of that makes symbolic execution fast and memory efficient. MXNet is portable and lightweight, scaling effectively to multiple GPUs and multiple machines. Support for Python, R, Julia, Scala, Go, Javascript and more.

[AutoGluon](https://autogluon.mxnet.io/index.html) is toolkit for Deep learning that automates machine learning tasks enabling you to easily achieve strong predictive performance in your applications. With just a few lines of code, you can train and deploy high-accuracy deep learning models on tabular, image, and text data.

[Anaconda](https://www.anaconda.com/) is a very popular Data Science platform for machine learning and deep learning that enables users to develop models, train them, and deploy them.

[PlaidML](https://github.com/plaidml/plaidml) is an advanced and portable tensor compiler for enabling deep learning on laptops, embedded devices, or other devices where the available computing hardware is not well supported or the available software stack contains unpalatable license restrictions.

[OpenCV](https://opencv.org) is a highly optimized library with focus on real-time computer vision applications. The C++, Python, and Java interfaces support Linux, MacOS, Windows, iOS, and Android.

[Scikit-Learn](https://scikit-learn.org/stable/index.html) is a Python module for machine learning built on top of SciPy, NumPy, and matplotlib, making it easier to apply robust and simple implementations of many popular machine learning algorithms.

[Weka](https://www.cs.waikato.ac.nz/ml/weka/) is an open source machine learning software that can be accessed through a graphical user interface, standard terminal applications, or a Java API. It is widely used for teaching, research, and industrial applications, contains a plethora of built-in tools for standard machine learning tasks, and additionally gives transparent access to well-known toolboxes such as scikit-learn, R, and Deeplearning4j. 

[Theano](https://github.com/Theano/Theano) is a Python library that allows you to define, optimize, and evaluate mathematical expressions involving multi-dimensional arrays efficiently including tight integration with NumPy.

[nGraph](https://github.com/NervanaSystems/ngraph) is an open source C++ library, compiler and runtime for Deep Learning. The nGraph Compiler aims to accelerate developing AI workloads using any deep learning framework and deploying to a variety of hardware targets.It provides the freedom, performance, and ease-of-use to AI developers.

[Jupyter Notebook](https://jupyter.org/) is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. Jupyter is used widely in industries that do data cleaning and transformation, numerical simulation, statistical modeling, data visualization, data science, and machine learning.

## Online ML Learning Resources

[Machine Learning by Stanford University from Coursera](https://www.coursera.org/learn/machine-learning)

[Machine Learning Courses Online from Coursera](https://www.coursera.org/courses?query=machine%20learning&)

[Machine Learning Courses Online from Udemy](https://www.udemy.com/topic/machine-learning/)

[Learn Machine Learning with Online Courses and Classes from edX](https://www.edx.org/learn/machine-learning)

# Robotics

[Back to the Top](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/96352533-b55fb380-1078-11eb-874c-f165cbcce899.png">
</p>

## Tools for Robotics

[ROS](https://www.ros.org/) is robotics middleware. Although ROS is not an operating system, it provides services designed for a heterogeneous computer cluster such as hardware abstraction, low-level device control, implementation of commonly used functionality, message-passing between processes, and package management.

[ROS2](https://index.ros.org/doc/ros2/) is a set of [software libraries and tools](https://github.com/ros2) that help you build robot applications. From drivers to state-of-the-art algorithms, and with powerful developer tools, ROS has what you need for your next robotics project. And it’s all open source.

[Robot Framework](https://robotframework.org/) is a generic open source automation framework. It can be used for test automation and robotic process automation. It has easy syntax, utilizing human-readable keywords. Its capabilities can be extended by libraries implemented with Python or Java. 

[The Robotics Library (RL)](https://github.com/roboticslibrary/rl) is a self-contained C++ library for robot kinematics, motion planning and control. It covers mathematics, kinematics and dynamics, hardware abstraction, motion planning, collision detection, and visualization.RL runs on many different systems, including Linux, macOS, and Windows. It uses CMake as a build system and can be compiled with Clang, GCC, and Visual Studio.

[MoveIt](https://moveit.ros.org/) is the most widely used software for manipulation and has been used on over 100 robots. It provides an easy-to-use robotics platform for developing advanced applications, evaluating new designs and building integrated products for industrial, commercial, R&D, and other domains.

[AutoGluon](https://autogluon.mxnet.io/index.html) is toolkit for [Deep learning](https://gitlab.com/maos20008/intro-to-machine-learning) that automates machine learning tasks enabling you to easily achieve strong predictive performance in your applications. With just a few lines of code, you can train and deploy high-accuracy deep learning models on tabular, image, and text data.

[Gazebo](http://gazebosim.org/) accurately and efficiently simulates indoor and outdoor robots. You get a robust physics engine, high-quality graphics, and programmatic and graphical interfaces.

[Robotics System Toolbox](https://www.mathworks.com/products/robotics.html) provides tools and algorithms for designing, simulating, and testing manipulators, mobile robots, and humanoid robots. For manipulators and humanoid robots, the toolbox includes algorithms for collision checking, trajectory generation, forward and inverse kinematics, and dynamics using a rigid body tree representation. 
For mobile robots, it includes algorithms for mapping, localization, path planning, path following, and motion control. The toolbox provides reference examples of common industrial robot applications. It also includes a library of 
commercially available industrial robot models that you can import, visualize, and simulate.

[Intel Robot DevKit](https://github.com/intel/robot_devkit) is the tool to generate Robotics Software Development Kit (RDK) designed for autonomous devices, including the ROS2 core and capacibilities packages like perception, planning, control driver etc. It provides flexible build/runtime configurations to meet different autonomous requirement on top of diversity hardware choices, for example use different hareware engine CPU/GPU/VPU to accelerate AI related features.

[Arduino](https://www.arduino.cc/) is an open-source platform used for building electronics projects. Arduino consists of both a physical programmable circuit board (often referred to as a microcontroller) and a piece of software, or IDE (Integrated Development Environment) that runs on your computer, used to write and upload computer code to the physical board.

[ArduPilot](https://ardupilot.org/ardupilot/index.html) enables the creation and use of trusted, autonomous, unmanned vehicle systems for the peaceful benefit of all. ArduPilot provides a comprehensive suite of tools suitable for almost any vehicle and application.

[AirSim](https://github.com/Microsoft/AirSim) is a simulator for drones, cars and more, built on Unreal Engine (we now also have an experimental Unity release). It is open-source, cross platform, and supports hardware-in-loop with popular flight controllers such as PX4 for physically and visually realistic simulations.

[F´ (F Prime)](https://github.com/nasa/fprime) is a component-driven framework that enables rapid development and deployment of spaceflight and other embedded software applications. Originally developed at the Jet Propulsion Laboratory, F´ has been successfully deployed on several space applications.

[The JPL Open Source Rover](https://github.com/nasa-jpl/open-source-rover) is an open source, build it yourself, scaled down version of the 6 wheel rover design that JPL uses to explore the surface of Mars. The Open Source Rover is designed almost entirely out of consumer off the shelf (COTS) parts. This project is intended to be a teaching and learning experience for those who want to get involved in mechanical engineering, software, electronics, or robotics.

[Light Detection and Ranging(LiDAR)](https://en.wikipedia.org/wiki/Lidar) is a remote sensing method that uses light in the form of a pulsed laser at an object, and uses the time and wavelength of the reflected beam of light to estimate the distance and in some applications ([Laser Imaging](https://en.wikipedia.org/wiki/Laser_scanning)), to create a 3D representation of the object and its surface characteristics. This technology is commonly used in aircraft and self-driving vehicles.

[AliceVision](https://github.com/alicevision/AliceVision) is a Photogrammetric Computer Vision Framework which provides a 3D Reconstruction and Camera Tracking algorithms. AliceVision aims to provide strong software basis with state-of-the-art computer vision algorithms that can be tested, analyzed and reused. The project is a result of collaboration between academia and industry to provide cutting-edge algorithms with the robustness and the quality required for production usage.

[CARLA](https://github.com/carla-simulator/carla) is an open-source simulator for autonomous driving research. CARLA has been developed from the ground up to support development, training, and validation of autonomous driving systems. In addition to open-source code and protocols, CARLA provides open digital assets (urban layouts, buildings, vehicles) that were created for this purpose and can be used freely. The simulation platform supports flexible specification of sensor suites and environmental conditions.

[ROS bridge](https://github.com/carla-simulator/ros-bridge) is a package to bridge ROS for CARLA Simulator.

[ROS-Industrial](https://rosindustrial.org/) is an open source project that extends the advanced capabilities of ROS software to manufacturing.

[AWS RoboMaker](https://aws.amazon.com/robomaker/) is the most complete cloud solution for robotic developers to simulate, test and securely deploy robotic applications at scale. RoboMaker provides a fully-managed, scalable infrastructure for simulation that customers use for multi-robot simulation and CI/CD integration with regression testing in simulation.

[Microsoft Robotics Developer Studio](https://www.microsoft.com/en-us/download/details.aspx?id=29081)  is a free .NET-based programming environment for building robotics applications. 

[Visual Studio Code Extension for ROS](https://github.com/ms-iot/vscode-ros) is an extension provides support for Robot Operating System (ROS) development.

[Azure Kinect ROS Driver](https://github.com/microsoft/azure_kinect_ros_driver) is a node which publishes sensor data from the [Azure Kinect Developer Kit](https://azure.microsoft.com/en-us/services/kinect-dk/) to the [Robot Operating System (ROS)](http://www.ros.org/). Developers working with ROS can use this node to connect an Azure Kinect Developer Kit to an existing ROS installation.

[Azure IoT Hub for ROS](https://github.com/microsoft/ros_azure_iothub) is a ROS package works with the Microsoft Azure IoT Hub service to relay telemetry messages from the Robot to Azure IoT Hub or reflect properties from the Digital Twin to the robot using dynamic reconfigure.

[ROS 2 with ONNX Runtime](https://github.com/ms-iot/ros_msft_onnx) is a program that uses ROS 2 to run on different hardware platforms using their respective AI acceleration libraries for optimized execution of the ONNX model.

[Azure Cognitive Services LUIS ROS Node](https://github.com/ms-iot/ros_msft_luis) is a ROS node that bridges between ROS and the Azure Language Understanding Service. it can be configured to process audio directly from a microphone, or can subscribe to a ROS audio topic, then processes speech and generates "intent" ROS messages which can be processed by another ROS node to generate ROS commands. 

## Robotics Learning Resources

[Robotics courses from Coursera](https://www.edx.org/learn/robotics)

[Learn Robotics with Online Courses and Classes from edX](https://www.edx.org/learn/robotics)

[Top Robotics Courses Online from Udemy](https://www.udemy.com/topic/robotics/)

[Free Online AI & Robotics Courses](https://www.futurelearn.com/subjects/it-and-computer-science-courses/ai-and-robotics)

[REC Foundation Robotics Industry Certification](https://www.roboticseducation.org/industry-certifications/)

[Carnegie Mellon Robotics Academy](https://www.cmu.edu/roboticsacademy/Training/Certifications.html)

[RIA Robotic Integrator Certification Program](https://www.robotics.org/robotics/integrator-certification)

[AWS RoboMaker – Develop, Test, Deploy, and Manage Intelligent Robotics Apps](https://aws.amazon.com/blogs/aws/aws-robomaker-develop-test-deploy-and-manage-intelligent-robotics-apps/)

[Microsoft AI School](https://aischool.microsoft.com/en-us/home)

[Language Understanding (LUIS) for Azure Cognitive Services](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/what-is-luis)

[Azure VM templates to bootstrap ROS and ROS 2 environments](https://ms-iot.github.io/ROSOnWindows/ROSAtMS/AzureVM.html)

[Google Robotics Research](https://research.google/teams/brain/robotics/)

# Networking

[Back to the Top](https://github.com/mikeroyal/RISC-V-Guide/blob/main/README.md#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/82833053-d1687b80-9e71-11ea-8c6d-074100f2f54b.png">
  <br />
</p>

## Networking Learning Resources
  
[AWS Certified Security - Specialty Certification](https://aws.amazon.com/certification/certified-security-specialty/)

[Microsoft Certified: Azure Security Engineer Associate](https://docs.microsoft.com/en-us/learn/certifications/azure-security-engineer)

[Google Cloud Certified Professional Cloud Security Engineer](https://cloud.google.com/certification/cloud-security-engineer)

[Cisco Security Certifications](https://www.cisco.com/c/en/us/training-events/training-certifications/certifications/security.html)

[The Red Hat Certified Specialist in Security: Linux](https://www.redhat.com/en/services/training/ex415-red-hat-certified-specialist-security-linux-exam)

[Linux Professional Institute LPIC-3 Enterprise Security Certification](https://www.lpi.org/our-certifications/lpic-3-303-overview)

[Cybersecurity Training and Courses from IBM Skills](https://www.ibm.com/skills/topics/cybersecurity/)

[Cybersecurity Courses and Certifications by Offensive Security](https://www.offensive-security.com/courses-and-certifications/)  
  
[Citrix Certified Associate – Networking(CCA-N)](http://training.citrix.com/cms/index.php/certification/networking/)

[Citrix Certified Professional – Virtualization(CCP-V)](https://www.globalknowledge.com/us-en/training/certification-prep/brands/citrix/section/virtualization/citrix-certified-professional-virtualization-ccp-v/)

[CCNP Routing and Switching](https://learningnetwork.cisco.com/s/ccnp-enterprise)

[Certified Information Security Manager(CISM)](https://www.isaca.org/credentialing/cism)

[Wireshark Certified Network Analyst (WCNA)](https://www.wiresharktraining.com/certification.html)

[Juniper Networks Certification Program Enterprise (JNCP)](https://www.juniper.net/us/en/training/certification/)

[Networking courses and specializations from Coursera](https://www.coursera.org/browse/information-technology/networking)

[Network & Security Courses from Udemy](https://www.udemy.com/courses/it-and-software/network-and-security/)

[Network & Security Courses from edX](https://www.edx.org/learn/cybersecurity)
  
  ## Tools & Networking Concepts
  
    • Connection: In networking, a connection refers to pieces of related information that are transferred through a network. This generally infers that a connection is built before the data transfer (by following the procedures laid out in a protocol) and then is deconstructed at the at the end of the data transfer.
    
    • Packet: A packet is, generally speaking, the most basic unit that is transferred over a network. When communicating over a network, packets are the envelopes that carry your data (in pieces) from one end point to the other.
    
Packets have a header portion that contains information about the packet including the source and destination, timestamps, network hops. The main portion of a packet contains the actual data being transferred. It is sometimes called the body or the payload.

    • Network Interface: A network interface can refer to any kind of software interface to networking hardware. For instance, if you have two network cards in your computer, you can control and configure each network interface associated with them individually.
    
A network interface may be associated with a physical device, or it may be a representation of a virtual interface. The "loop-back" device, which is a virtual interface to the local machine, is an example of this.

    • LAN: LAN stands for "local area network". It refers to a network or a portion of a network that is not publicly accessible to the greater internet. A home or office network is an example of a LAN.
    
    • WAN: WAN stands for "wide area network". It means a network that is much more extensive than a LAN. While WAN is the relevant term to use to describe large, dispersed networks in general, it is usually meant to mean the internet, as a whole.
If an interface is connected to the WAN, it is generally assumed that it is reachable through the internet.

    • Protocol: A protocol is a set of rules and standards that basically define a language that devices can use to communicate. There are a great number of protocols in use extensively in networking, and they are often implemented in different layers. 
    
Some low level protocols are TCP, UDP, IP, and ICMP. Some familiar examples of application layer protocols, built on these lower protocols, are HTTP (for accessing web content), SSH, TLS/SSL, and FTP.

    • Port: A port is an address on a single machine that can be tied to a specific piece of software. It is not a physical interface or location, but it allows your server to be able to communicate using more than one application.
    
    • Firewall: A firewall is a program that decides whether traffic coming into a server or going out should be allowed. A firewall usually works by creating rules for which type of traffic is acceptable on which ports. Generally, firewalls block ports that are not used by a specific application on a server.
    
    • NAT: Network address translation is a way to translate requests that are incoming into a routing server to the relevant devices or servers that it knows about in the LAN. This is usually implemented in physical LANs as a way to route requests through one IP address to the necessary backend servers.
    
    • VPN: Virtual private network is a means of connecting separate LANs through the internet, while maintaining privacy. This is used as a means of connecting remote systems as if they were on a local network, often for security reasons.
    
## Network Layers

	While networking is often discussed in terms of topology in a horizontal way, between hosts, its implementation is layered in a vertical fashion throughout a computer or network. This means is that there are multiple technologies and protocols that are built on top of each other in order for communication to function more easily. Each successive, higher layer abstracts the raw data a little bit more, and makes it simpler to use for applications and users. It also allows you to leverage lower layers in new ways without having to invest the time and energy to develop the protocols and applications that handle those types of traffic.
 
	As data is sent out of one machine, it begins at the top of the stack and filters downwards. At the lowest level, actual transmission to another machine takes place. At this point, the data travels back up through the layers of the other computer. Each layer has the ability to add its own "wrapper" around the data that it receives from the adjacent layer, which will help the layers that come after decide what to do with the data when it is passed off.
 
	One method of talking about the different layers of network communication is the OSI model. OSI stands for Open Systems Interconnect.This model defines seven separate layers. The layers in this model are:

    • Application: The application layer is the layer that the users and user-applications most often interact with. Network communication is discussed in terms of availability of resources, partners to communicate with, and data synchronization.
    
    • Presentation: The presentation layer is responsible for mapping resources and creating context. It is used to translate lower level networking data into data that applications expect to see.
    
    • Session: The session layer is a connection handler. It creates, maintains, and destroys connections between nodes in a persistent way.
    
    • Transport: The transport layer is responsible for handing the layers above it a reliable connection. In this context, reliable refers to the ability to verify that a piece of data was received intact at the other end of the connection. This layer can resend information that has been dropped or corrupted and can acknowledge the receipt of data to remote computers.

    • Network: The network layer is used to route data between different nodes on the network. It uses addresses to be able to tell which computer to send information to. This layer can also break apart larger messages into smaller chunks to be reassembled on the opposite end.
    
    • Data Link: This layer is implemented as a method of establishing and maintaining reliable links between different nodes or devices on a network using existing physical connections.
    
    • Physical: The physical layer is responsible for handling the actual physical devices that are used to make a connection. This layer involves the bare software that manages physical connections as well as the hardware itself (like Ethernet).
    
The TCP/IP model, more commonly known as the Internet protocol suite, is another layering model that is simpler and has been widely adopted.It defines the four separate layers, some of which overlap with the OSI model:

    • Application: In this model, the application layer is responsible for creating and transmitting user data between applications. The applications can be on remote systems, and should appear to operate as if locally to the end user. 
The communication takes place between peers network.

    • Transport: The transport layer is responsible for communication between processes. This level of networking utilizes ports to address different services. It can build up unreliable or reliable connections depending on the type of protocol used.
    
    • Internet: The internet layer is used to transport data from node to node in a network. This layer is aware of the endpoints of the connections, but does not worry about the actual connection needed to get from one place to another. IP addresses are defined in this layer as a way of reaching remote systems in an addressable manner.
    
    • Link: The link layer implements the actual topology of the local network that allows the internet layer to present an addressable interface. It establishes connections between neighboring nodes to send data.
    
## Interfaces
Interfaces are networking communication points for your computer. Each interface is associated with a physical or virtual networking device. Typically, your server will have one configurable network interface for each Ethernet or wireless internet card you have. In addition, it will define a virtual network interface called the "loopback" or localhost interface. This is used as an interface to connect applications and processes on a single computer to other applications and processes. You can see this referenced as the "lo" interface in many tools.

## Protocols
Networking works by piggybacks on a number of different protocols on top of each other. In this way, one piece of data can be transmitted using multiple protocols encapsulated within one another.

Media access control is a communications protocol that is used to distinguish specific devices. Each device is supposed to get a unique MAC address during the manufacturing process that differentiates it from every other device on the internet. Addressing hardware by the MAC address allows you to reference a device by a unique value even when the software on top may change the name for that specific device during operation. Media access control is one of the only protocols from the link layer that you are likely to interact with on a regular basis.

The IP protocol is one of the fundamental protocols that allow the internet to work. IP addresses are unique on each network and they allow machines to address each other across a network. It is implemented on the internet layer in the IP/TCP model. Networks can be linked together, but traffic must be routed when crossing network boundaries. This protocol assumes an unreliable network and multiple paths to the same destination that it can dynamically change between. There are a number of different implementations of the protocol. The most common implementation today is IPv4, although IPv6 is growing in popularity as an alternative due to the scarcity of IPv4 addresses available and improvements in the protocols capabilities.

ICMP: internet control message protocol is used to send messages between devices to indicate the availability or error conditions. These packets are used in a variety of network diagnostic tools, such as ping and traceroute. Usually ICMP packets are transmitted when a packet of a different kind meets some kind of a problem. Basically, they are used as a feedback mechanism for network communications.

TCP: Transmission control protocol is implemented in the transport layer of the IP/TCP model and is used to establish reliable connections. TCP is one of the protocols that encapsulates data into packets. It then transfers these to the remote end of the connection using the methods available on the lower layers. On the other end, it can check for errors, request certain pieces to be resent, and reassemble the information into one logical piece to send to the application layer. The protocol builds up a connection prior to data transfer using a system called a three-way handshake. This is a way for the two ends of the communication to acknowledge the request and agree upon a method of ensuring data reliability. After the data has been sent, the connection is torn down using a similar four-way handshake. TCP is the protocol of choice for many of the most popular uses for the internet, including WWW, FTP, SSH, and email. It is safe to say that the internet we know today would not be here without TCP.

UDP: User datagram protocol is a popular companion protocol to TCP and is also implemented in the transport layer. The fundamental difference between UDP and TCP is that UDP offers unreliable data transfer. It does not verify that data has been received on the other end of the connection. This might sound like a bad thing, and for many purposes, it is. However, it is also extremely important for some functions. It’s not required to wait for confirmation that the data was received and forced to resend data, UDP is much faster than TCP. It does not establish a connection with the remote host, it simply fires off the data to that host and doesn't care if it is accepted or not. Since UDP is a simple transaction, it is useful for simple communications like querying for network resources. It also doesn't maintain a state, which makes it great for transmitting data from one machine to many real-time clients. This makes it ideal for VOIP, games, and other applications that cannot afford delays.

HTTP: Hypertext transfer protocol is a protocol defined in the application layer that forms the basis for communication on the web. HTTP defines a number of functions that tell the remote system what you are requesting. For instance, GET, POST, and DELETE all interact with the requested data in a different way.

[JSON Web Token (JWT)](https://jwt.io) is a compact URL-safe means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is digitally signed using JSON Web Signature (JWS).

[OAuth 2.0](https://oauth.net/2/) is an open source authorization framework that enables applications to obtain limited access to user accounts on an HTTP service, such as Amazon, Google, Facebook, Microsoft, Twitter GitHub, and DigitalOcean. It works by delegating user authentication to the service that hosts the user account, and authorizing third-party applications to access the user account.

FTP: File transfer protocol is in the application layer and provides a way of transferring complete files from one host to another. It is inherently insecure, so it is not recommended for any externally facing network unless it is implemented as a public, download-only resource.

DNS: Domain name system is an application layer protocol used to provide a human-friendly naming mechanism for internet resources. It is what ties a domain name to an IP address and allows you to access sites by name in your browser.

SSH: Secure shell is an encrypted protocol implemented in the application layer that can be used to communicate with a remote server in a secure way. Many additional technologies are built around this protocol because of its end-to-end encryption and ubiquity. There are many other protocols that we haven't covered that are equally important. However, this should give you a good overview of some of the fundamental technologies that make the internet and networking possible.

## Virtualization

[KVM (for Kernel-based Virtual Machine)](https://www.linux-kvm.org/page/Main_Page) is a full virtualization solution for Linux on x86 hardware containing virtualization extensions (Intel VT or AMD-V). It consists of a loadable kernel module, kvm.ko, that provides the core virtualization infrastructure and a processor specific module, kvm-intel.ko or kvm-amd.ko.

[QEMU](https://www.qemu.org) is a fast processor emulator using a portable dynamic translator. QEMU emulates a full system, including a processor and various peripherals. It can be used to launch a different Operating System without rebooting the PC or to debug system code.

[Hyper-V](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/) enables running virtualized computer systems on top of a physical host. These virtualized systems can be used and managed just as if they were physical computer systems, however they exist in virtualized and isolated environment. Special software called a hypervisor manages access between the virtual systems and the physical hardware resources. Virtualization enables quick deployment of computer systems, a way to quickly restore systems to a previously known good state, and the ability to migrate systems between physical hosts.

[VirtManager](https://github.com/virt-manager/virt-manager) is a graphical tool for managing virtual machines via libvirt. Most usage is with QEMU/KVM virtual machines, but Xen and libvirt LXC containers are well supported. Common operations for any libvirt driver should work.

[oVirt](https://www.ovirt.org) is an open-source distributed virtualization solution, designed to manage your entire enterprise infrastructure. oVirt uses the trusted KVM hypervisor and is built upon several other community projects, including libvirt, Gluster, PatternFly, and Ansible.Founded by Red Hat as a community project on which Red Hat Enterprise Virtualization is based allowing for centralized management of virtual machines, compute, storage and networking resources, from an easy-to-use web-based front-end with platform independent access.

[Xen](https://github.com/xen-project/xen) is focused on advancing virtualization in a number of different commercial and open source applications, including server virtualization, Infrastructure as a Services (IaaS), desktop virtualization, security applications, embedded and hardware appliances, and automotive/aviation.

[Ganeti](https://github.com/ganeti/ganeti) is a virtual machine cluster management tool built on top of existing virtualization technologies such as Xen or KVM and other open source software. Once installed, the tool assumes management of the virtual instances (Xen DomU).

[Packer](https://www.packer.io/) is an open source tool for creating identical machine images for multiple platforms from a single source configuration. Packer is lightweight, runs on every major operating system, and is highly performant, creating machine images for multiple platforms in parallel. Packer does not replace configuration management like Chef or Puppet. In fact, when building images, Packer is able to use tools like Chef or Puppet to install software onto the image.

[Vagrant](https://www.vagrantup.com/) is a tool for building and managing virtual machine environments in a single workflow. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases production parity, and makes the "works on my machine" excuse a relic of the past. It provides easy to configure, reproducible, and portable work environments built on top of industry-standard technology and controlled by a single consistent workflow to help maximize the productivity and flexibility of you and your team.

## Contribute

- [x] If would you like to contribute to this guide simply make a [Pull Request](https://github.com/mikeroyal/RISC-V-Guide/pulls).


## License

[Back to the Top](https://github.com/mikeroyal/risc-v-Guide/blob/main/README.md#table-of-contents)

Distributed under the [Creative Commons Attribution 4.0 International (CC BY 4.0) Public License](https://creativecommons.org/licenses/by/4.0/).
