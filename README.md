# Awesome Radio [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Ham radio resources with an emphasis on station automation, high-performance antennas, and high impact, hard to find gems of information. Covering everything from Technician through Extra class and beyond.

## Contents

- [Station Automation](#station-automation)
  - [Flex 6400M and SmartSDR](#flex-6400m-and-smartsdr)
  - [Elecraft](#elecraft)
  - [SPE Expert Amplifiers](#spe-expert-amplifiers)
  - [Elecraft Amplifiers and Tuners](#elecraft-amplifiers-and-tuners)
  - [SteppIR Antennas](#steppir-antennas)
  - [Multi-Rig Integration and Control](#multi-rig-integration-and-control)
- [Antennas, Feedlines and RF](#antennas-feedlines-and-rf)
  - [Verticals and Phased Arrays](#verticals-and-phased-arrays)
  - [Chokes and Common-Mode Current](#chokes-and-common-mode-current)
  - [Feedline Selection and Loss](#feedline-selection-and-loss)
  - [Antenna Modeling](#antenna-modeling)
- [SDR and Signal Processing](#sdr-and-signal-processing)
- [Digital Modes](#digital-modes)
- [GitHub Projects](#github-projects)
- [Logging and Contesting](#logging-and-contesting)
- [Licensing and Learning](#licensing-and-learning)

---

## Station Automation

### Flex 6400M and SmartSDR

- [FlexRadio Systems](https://www.flexradio.com) - Manufacturer of the Flex 6400M and SmartSDR software-defined radio platform.
- [FlexRadio Community Forums](https://community.flexradio.com) - Official community forums covering SmartSDR, API usage, hardware, and station integration.
- [SmartSDR API Documentation](https://documentation.flexradio.com) - Official REST and TCP API reference for programmatic control of SmartSDR-based radios.
- [SmartSDR for Mac](https://www.flexradio.com/ssdr-for-mac/) - Native macOS client for SmartSDR, with DAX audio routing and CAT support.
- [DAX (Digital Audio eXchange)](https://www.flexradio.com/downloads/) - Virtual audio routing layer for SmartSDR enabling integration with logging, digital mode, and audio processing software.
- [SmartLink](https://www.flexradio.com/smartlink/) - Remote access system allowing full SmartSDR operation over the internet with low latency.

### Elecraft

- [Elecraft](https://www.elecraft.com) - Manufacturer of the K3, KX2, and related accessories; documentation and firmware downloads available.
- [elecraft-docs](https://github.com/radiolabme/elecraft-docs) - Curated technical documentation, automation notes, and configuration references for Elecraft K3 and KX2 operators.
- [Elecraft Mailing List Archives](https://mailman.qth.net/pipermail/elecraft/) - Decades of operator experience, modification tips, and troubleshooting in searchable archive form.
- [K3 Programmer](https://www.k3programmer.com) - Third-party configuration and band-data management tool for the Elecraft K3 and K3S.

### SPE Expert Amplifiers

- [SPE Expert](https://www.spe-expert.com) - Manufacturer of the Expert 1.3K-FA and related solid-state amplifiers; manuals and firmware updates available.
- [SPE Expert 1.3K-FA Manual](https://www.spe-expert.com/wp-content/uploads/2020/01/Expert_1.3K-FA_Manual.pdf) - Full operator manual covering serial CAT interface, automation inputs, and band-data connector pinout.
- [SPE Support Forum](https://www.spe-expert.com/forum/) - Official forum with firmware announcements and operator-contributed automation scripts.

### Elecraft Amplifiers and Tuners

- [KPA500 Operator's Manual](https://www.elecraft.com/Downloads/KPA500%20Ops%20Manual.pdf) - Serial interface reference and automation pinout for the Elecraft KPA500 solid-state amplifier.
- [KAT500 Operator's Manual](https://www.elecraft.com/Downloads/KAT500%20Ops%20Manual.pdf) - Serial control protocol and automation notes for the Elecraft KAT500 automatic antenna tuner.
- [KPA1500 Operator's Manual](https://www.elecraft.com/Downloads/KPA1500%20Ops%20Manual.pdf) - Serial and Ethernet interface documentation for the Elecraft KPA1500 amplifier, useful reference for KPA500 operators.
- [Elecraft Programmer's Reference](https://www.elecraft.com/Downloads/K3%20Programmer's%20Reference.pdf) - Comprehensive CAT command reference covering K3, KPA500, KAT500, and accessory control.

### SteppIR Antennas

- [SteppIR Antennas](https://www.steppir.com) - Manufacturer of motorized, continuously tunable antennas including the BigIR vertical and SDA100 controller.
- [SDA100 Quick Start Guide](https://www.steppir.com/wp-content/uploads/2019/02/SDA100-Quick-Start-Guide.pdf) - Setup and calibration guide for the SDA100 antenna controller used with BigIR and other SteppIR elements.
- [SteppIR EHF Interface](https://www.steppir.com/products/sda100/) - Description of the EHF (Extended High Frequency) interface allowing CAT-controlled antenna tuning from logging and contest software.
- [SteppIR User Group](https://groups.io/g/steppir) - Active operator community covering installation, troubleshooting, automation, and calibration of SteppIR antennas.

### Multi-Rig Integration and Control

- [Hamlib](https://hamlib.github.io) - Open-source radio control library providing a unified API for dozens of transceivers and rotators; the backbone of most amateur radio automation software.
- [rigctld](https://manpages.ubuntu.com/manpages/jammy/man8/rigctld.8.html) - Network daemon from Hamlib exposing rig control over TCP; enables multiple applications to share control of one radio simultaneously.
- [flrig](https://sourceforge.net/projects/fldigi/files/flrig/) - Lightweight rig control application from the fldigi suite; pairs with fldigi and supports band/mode/frequency automation.
- [N1MM+ Logger](https://n1mmwireless.com) - The dominant Windows contest logging application with deep CAT integration, SO2R support, and band-data relay output for amplifier and antenna switching.
- [Logger32](https://www.logger32.net) - Full-featured DX logging application with multi-rig CAT control, cluster integration, and antenna switching relay outputs.
- [OmniRig](http://www.dxatlas.com/OmniRig/) - Windows COM-based rig control engine that allows multiple applications to share a single CAT connection to a transceiver.
- [Band Decoder MK2](https://github.com/ok1rr/BandDecoderMK2) - Open-source Arduino-based band decoder that reads frequency from CAT and drives antenna switches, amplifier band inputs, and SteppIR controllers.

---

## Antennas, Feedlines and RF

### Verticals and Phased Arrays

- [ON4UN's Low-Band DXing](https://www.qth.com/on4un/) - The definitive reference for low-band vertical and phased array design, modeling, and installation.
- [DX Engineering Phased Array Systems](https://www.dxengineering.com/techarticles/DXE-TECH-PHASED.pdf) - Technical overview of two-element phased vertical arrays with practical construction details.
- [4O3A Antenna Systems](https://www.4o3a.com) - Operator-authored resources on high-performance vertical and beam antenna systems with real-world measurement data.
- [The ARRL Antenna Book](https://www.arrl.org/arrl-antenna-book) - Comprehensive reference covering vertical, wire, and phased array antennas with modeling examples.

### Chokes and Common-Mode Current

- [W8JI Choke and Common-Mode Resources](https://www.w8ji.com/common_mode_current.htm) - Tom Rauch's deeply researched pages on common-mode current, choke design, and RF grounding — among the most cited practical references on the subject.
- [K9YC RFI, Ferrites, and Common Mode Chokes](http://audiosystemsgroup.com/RFI-Ham.pdf) - Jim Brown's comprehensive guide to ferrite materials, choke construction, and common-mode suppression for ham stations.
- [Palomar Engineers Ferrite Toroid Calculator](https://www.palomar-engineers.com/ferrite-toroids/ferrite-toroid-design-calculator/) - Online calculator for choke impedance given core material, winding count, and frequency.
- [Fair-Rite Ferrite Products](https://www.fair-rite.com) - Primary ferrite core manufacturer; datasheets and material characteristic curves for Mix 31, 43, 61, and 75 used in ham choke construction.
- [Ugly Balun / Choke Construction](https://www.w8ji.com/ugly_balun.htm) - W8JI's measured analysis of the common "ugly balun" feedline choke showing when it works and when it fails.

### Feedline Selection and Loss

- [Times Microwave LMR Cable](https://www.timesmicrowave.com/lmr) - Industry-standard flexible coaxial cable; manufacturer's loss tables and technical specifications for LMR-400, LMR-600, and LMR-900 series.
- [The Cable Company Coax Loss Calculator](https://www.timesmicrowave.com/calculator) - Times Microwave online tool for calculating dB loss at frequency for all LMR cable types by run length.
- [DX Engineering RG-6 and Hardline Resources](https://www.dxengineering.com/search/department/coaxial-cable) - Commercial-grade feedline options including CATV hardline adaptations popular for high-power installations.
- [VK1OD Transmission Line Details](https://owenduffy.net/calc/tld.htm) - Owen Duffy's online transmission line calculator covering matched and mismatched loss, SWR, and impedance transformation.

### Antenna Modeling

- [4nec2](https://www.qsl.net/4nec2/) - Free Windows NEC2/NEC4 antenna modeling application with a visual geometry editor and far-field pattern display; the most accessible entry point for numerical antenna modeling.
- [EZNEC](https://eznec.com) - Roy Lewallen's widely used Windows antenna modeling program based on NEC2; supports up to 500 wires and is standard for most published amateur antenna designs.
- [OpenEMS](https://www.openems.de) - Open-source finite-difference time-domain (FDTD) electromagnetic field solver; handles complex structures including coax feeds, shields, and PCB antennas beyond NEC's wire-only limitations.
- [MMANA-GAL](http://gal-ana.de/basicmm/en/) - Free antenna modeling software based on the moment method, popular for its simple interface and good accuracy for wire antennas.
- [Antenna Model](https://www.antennamodel.com) - Commercial NEC-based modeling application with an active developer, good for EZNEC users seeking an alternative with updated NEC4 support.

---

## SDR and Signal Processing

---

## Digital Modes

---

## GitHub Projects

---

## Logging and Contesting

---

## Licensing and Learning
