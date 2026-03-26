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

- [SDR++](https://www.sdrpp.org) - Cross-platform SDR receiver with a clean interface, broad hardware support (RTL-SDR, HackRF, Airspy, LimeSDR), and a plugin architecture.
- [SDRangel](https://github.com/f4exb/sdrangel) - Qt-based SDR and signal analyzer with transmit capability, extensive plugin ecosystem, and support for Flex radios via SmartSDR protocol.
- [GQRX](https://gqrx.dk) - GNU Radio-based SDR receiver with a straightforward interface; well-suited for spectrum monitoring and audio demodulation on Linux and macOS.
- [CubicSDR](https://cubicsdr.com) - Cross-platform SDR application built on liquid-dsp and SoapySDR; integrates with Flex radios via IQ data.
- [GNU Radio](https://www.gnuradio.org) - Open-source signal processing toolkit and flow-graph development environment used to build custom SDR applications, demodulators, and analysis tools.
- [SoapySDR](https://github.com/pothosware/SoapySDR) - Vendor-neutral hardware abstraction layer for SDR devices; the common substrate used by SDR++, CubicSDR, and many other applications to support multiple hardware backends.
- [RTL-SDR Blog](https://www.rtl-sdr.com) - Extensive tutorials, software guides, and project write-ups covering RTL-SDR and a wide range of SDR applications.

---

## Digital Modes

- [WSJT-X](https://wsjt.sourceforge.io/wsjtx.html) - The reference implementation of FT8, FT4, MSK144, and other weak-signal modes; standard software for modern DX and contest operating.
- [JS8Call](https://js8call.com) - Conversational messaging protocol built on the JS8 mode (derived from FT8) for keyboard-to-keyboard QSOs at weak signal levels.
- [fldigi](http://www.w1hkj.com) - Mature multi-mode digital modem supporting PSK31, RTTY, Olivia, THOR, and dozens of others; integrates with flrig for rig control.
- [VARA HF](https://www.winlink.org/VARAHF) - High-performance adaptive HF modem used by Winlink and JS8Call; significantly outperforms older PACTOR modems at comparable price.
- [Winlink](https://www.winlink.org) - Email-over-radio network supporting HF, VHF, and satellite links; widely used for emergency communications and DX email.
- [JTDX](https://jtdx.tech) - Fork of WSJT-X with enhanced weak signal decoding algorithms; popular for difficult DX paths.
- [GridTracker](https://gridtracker.org) - Real-time map overlay for WSJT-X showing decoded callsigns, grid squares, and propagation paths.

---

## GitHub Projects

- [Hamlib](https://github.com/Hamlib/Hamlib) - The standard open-source library for rig and rotator control; supports hundreds of radios via a unified API used by nearly every ham automation tool.
- [flrig](https://github.com/w1hkj/flrig) - Rig control front-end from the fldigi suite; lightweight, cross-platform, and paired tightly with fldigi for digital mode use.
- [Band Decoder MK2](https://github.com/ok1rr/BandDecoderMK2) - Arduino-based band decoder reading CAT frequency and driving antenna switch, amp band-data, and SteppIR controller outputs.
- [SDRangel](https://github.com/f4exb/sdrangel) - Full-featured SDR transceiver application with Flex SmartSDR protocol support and an extensive signal processing plugin ecosystem.
- [SoapySDR](https://github.com/pothosware/SoapySDR) - Hardware abstraction layer enabling SDR software to support many different hardware backends through a common API.
- [OpenEMS](https://github.com/thliebig/openEMS) - FDTD electromagnetic field solver for antenna and RF structure simulation beyond NEC's wire-antenna scope.
- [pyhamtools](https://github.com/dh1tw/pyhamtools) - Python library for callsign lookup, log analysis, grid square calculations, and other common ham radio data operations.
- [ham2mon](https://github.com/madengr/ham2mon) - SDR-based multi-channel scanner and recorder for monitoring amateur and public safety bands.

---

## Logging and Contesting

- [N1MM+ Logger](https://n1mmwireless.com) - The most widely used Windows contest logging application; supports SO2R, deep CAT integration, and band-data relay for amplifier and antenna automation.
- [Logger32](https://www.logger32.net) - Feature-rich DX logging application with multi-rig CAT control, DX cluster integration, and relay-based antenna switching outputs.
- [DXLab Suite](https://www.dxlabsuite.com) - Integrated suite of Windows applications covering logging, propagation, DX spotting, rig control, and antenna rotator management.
- [Log4OM](https://www.log4om.com) - Modern cross-platform amateur radio logging application with built-in DX cluster, LOTW/eQSL integration, and CAT rig control.
- [LOTW (Logbook of the World)](https://lotw.arrl.org) - ARRL's electronic QSL and award confirmation system; the standard for DXCC, WAS, and most major award tracking.
- [ClubLog](https://clublog.org) - Web-based log upload and analysis platform with OQRS (online QSL request), DX expedition log search, and propagation statistics.
- [eQSL](https://eqsl.cc) - Electronic QSL card exchange network accepted for some awards programs; an alternative to paper QSLs with fast confirmations.

---

## Licensing and Learning

- [HamStudy](https://hamstudy.org) - Free online question pool study tool for Technician, General, and Amateur Extra exams with spaced-repetition flashcard mode.
- [ARRL](https://www.arrl.org) - The American Radio Relay League; publishes the FCC question pools, exam prep books, and the ARRL Handbook — the field's primary technical reference.
- [FCC ULS (Universal Licensing System)](https://wireless.fcc.gov/uls/) - Official FCC database for license lookup, renewal, and application; required stop for all US amateur operators.
- [Gordon West Training](https://gordonwestradioschool.com) - Audio and book study materials for all license classes, widely recommended for structured exam preparation.
- [Ham Radio Prep](https://hamradioprep.com) - Modern online course platform with video instruction and practice exams for all three US license classes.
- [QRZ.com](https://www.qrz.com) - Callsign lookup database, logbook, forums, and a comprehensive learning center with license exam practice tests.
