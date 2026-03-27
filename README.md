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
- [FlexRadio Community Forums](https://community.flexradio.com) - Official community forums covering SmartSDR API usage, CAT integration, hardware, and station automation.
- [SmartSDR for Mac](https://www.flexradio.com/ssdr-for-mac/) - Native macOS client for SmartSDR, with DAX audio routing and CAT support.
- [nDAX](https://github.com/kc2g-flex-tools/nDAX) - Linux-native PulseAudio audio device for FlexRadio DAX slices, enabling SmartSDR audio integration without Windows or Maestro.
- [nCAT](https://github.com/kc2g-flex-tools/nCAT) - Exposes a Flex 6xxx radio as a hamlib/rigctld-compatible CAT interface on TCP, allowing any hamlib-aware application to control the radio on Linux.
- [FlexRadio SmartSDR Group](https://groups.io/g/FlexRadioSmartSDR) - Active community covering SmartSDR operation, peripherals, and third-party software integration including DDUtil and SliceMaster.

### Elecraft

- [Elecraft](https://www.elecraft.com) - Manufacturer of the K3, KX2, and related accessories; documentation and firmware downloads available.
- [elecraft-docs](https://github.com/radiolabme/elecraft-docs) - Curated technical documentation, automation notes, and configuration references for Elecraft K3 and KX2 operators.
- [Elecraft Mailing List Archives](https://mailman.qth.net/pipermail/elecraft/) - Decades of operator experience, modification tips, and troubleshooting in searchable archive form.
- [Elecraft Group](https://groups.io/g/elecraft) - Active discussion group covering all Elecraft radios including K4, K3S, K3, KX3, and KX2.

### SPE Expert Amplifiers

- [SPE Expert Amplifiers](https://www.spetlc.com) - Manufacturer of the Expert 1.3K-FA solid-state amplifier; firmware downloads, manuals, and support hosted at spetlc.com.
- [1.3K-FA User Manual (Third Series, Rev. 3.1)](https://www.spetlc.com/images/download/1.3K-FA/User.Manual.EXPERT.1.3K-FA-EN-rev.3.1.Third.Series.pdf) - Full operator manual covering ALC settings, serial CAT interface, band-data connector pinout, and antenna tuner integration.
- [Application Programmer's Guide](https://www.radioamatore.info/attachments/article/2134/Application-Programmers-Guide-1.3K-2K-1.1.pdf) - Serial protocol reference for automated control of the Expert 1.3K-FA and 2K-FA amplifiers, covering command syntax and status responses.
- [SPE Expert Amps Group](https://speexpertamps.groups.io/g/main) - Community of Expert amplifier owners covering firmware updates, troubleshooting, station integration, and automation scripts.
- [SPE Expert with Flex 6400M](https://community.flexradio.com/discussion/7941411/spe-expert-1-3k-fa-amp) - FlexRadio community thread on integrating the 1.3K-FA with SmartSDR, covering CAT interface configuration and band-data setup.

### Elecraft Amplifiers and Tuners

- [KPA500 Operator's Manual](https://www.elecraft.com/Downloads/KPA500%20Ops%20Manual.pdf) - Serial interface reference and automation pinout for the Elecraft KPA500 solid-state amplifier.
- [KAT500 Operator's Manual](https://www.elecraft.com/Downloads/KAT500%20Ops%20Manual.pdf) - Serial control protocol and automation notes for the Elecraft KAT500 automatic antenna tuner.
- [KPA1500 Operator's Manual](https://www.elecraft.com/Downloads/KPA1500%20Ops%20Manual.pdf) - Serial and Ethernet interface documentation for the Elecraft KPA1500 amplifier, useful reference for KPA500 operators.
- [Elecraft Programmer's Reference](https://www.elecraft.com/Downloads/K3%20Programmer's%20Reference.pdf) - Comprehensive CAT command reference covering K3, KPA500, KAT500, and accessory control.

### SteppIR Antennas

- [SteppIR Antennas](https://www.steppir.com) - Manufacturer of motorized, continuously tunable antennas including the BigIR vertical and SDA100 controller.
- [SteppIR Support Files](https://consumer.steppir.com/support/files/) - Official downloads page for SDA100 firmware, operator guides, and assembly documentation.
- [SDA100 Serial Interface Document (2021)](https://consumer.steppir.com/wp-content/uploads/2021/05/Updated-Serial-Interface-Document-2021.pdf) - Official serial interface specification covering Data In/Data Out pinout, operating configurations, and radio compatibility table.
- [SDA100 Serial Protocol Specification (2005)](https://www.wimo.com/media/manuals/STEPPIR/Steppir_Serial-interface-operation.pdf) - Complete low-level protocol document detailing the 11-byte command/response format, frequency encoding, and all Data Out command codes (set, home, calibrate, disable).
- [Controlling SDA100 from Python](https://www.la1k.no/2019/09/25/controlling-a-steppir-sda-100-controller-from-python/) - Practical protocol walkthrough by LA1K with Python code, byte-level frequency encoding analysis, and worked examples at 9600 baud.
- [bjorgan/steppir](https://github.com/bjorgan/steppir) - Python library providing a high-level API over the SDA100 Data Out serial port: frequency setting, direction control, homing, and calibration.
- [DXLab Commander SteppIR Integration](https://www.dxlabsuite.com/dxlabwiki/SteppIRFrequencyTracking) - DXLab wiki covering Commander's secondary CAT port configuration for SteppIR frequency tracking, protocol selection, and baud rate settings.
- [SteppIR User Group](https://groups.io/g/steppir) - Active owner community covering installation, troubleshooting, SDA100 automation, and calibration of all SteppIR antenna models.

### Multi-Rig Integration and Control

- [Hamlib](https://hamlib.github.io) - Open-source radio control library providing a unified API for dozens of transceivers and rotators; the backbone of most amateur radio automation software.
- [rigctld](https://github.com/Hamlib/Hamlib/wiki/Documentation) - Network daemon from Hamlib exposing rig control over TCP; enables multiple applications to share control of one radio simultaneously.
- [flrig](https://sourceforge.net/projects/fldigi/files/flrig/) - Lightweight rig control application from the fldigi suite; pairs with fldigi and supports band/mode/frequency automation.
- [N1MM+ Logger](https://n1mmwp.hamdocs.com/) - The dominant Windows contest logging application with deep CAT integration, SO2R support, and band-data relay output for amplifier and antenna switching.
- [Logger32](https://www.logger32.net) - Full-featured DX logging application with multi-rig CAT control, cluster integration, and antenna switching relay outputs.
- [OmniRig](https://www.dxatlas.com/OmniRig/) - Windows COM-based rig control engine that allows multiple applications to share a single CAT connection to a transceiver.
- [node-red-contrib-hamlib](https://github.com/stephenhouser/node-red-contrib-hamlib) - Node-RED nodes for Hamlib rig control via rigctld, enabling visual flow-based station automation.
- [Node-RED Ham Radio Group](https://groups.io/g/nodered-hamradio) - Community for sharing and collaborating on Node-RED flows for ham radio station control and automation.
- [Software Controlled Ham Radio Group](https://groups.io/g/SoftwareControlledHamRadio) - Broad community covering software-driven ham radio projects including CAT control, station automation, and SDR integration.

---

## Antennas, Feedlines and RF

### Verticals and Phased Arrays

- [DX Engineering Phased Array Systems](https://www.dxengineering.com/techarticles/DXE-TECH-PHASED.pdf) - Technical overview of two-element phased vertical arrays with practical construction details.
- [4O3A Antenna Systems](https://4o3a.com) - Operator-authored resources on high-performance vertical and beam antenna systems with real-world measurement data.
- [The ARRL Antenna Book](https://www.arrl.org/arrl-antenna-book) - Comprehensive reference covering vertical, wire, and phased array antennas with modeling examples.

### Chokes and Common-Mode Current

- [W8JI Choke and Common-Mode Resources](https://www.w8ji.com/common_mode_current.htm) - Tom Rauch's deeply researched pages on common-mode current, choke design, and RF grounding — among the most cited practical references on the subject.
- [K9YC RFI, Ferrites, and Common Mode Chokes](https://content-files.shure.com/KnowledgeBaseFiles/troubleshooting-rfi-jim-brown-ham.pdf) - Jim Brown's comprehensive guide to ferrite materials, choke construction, and common-mode suppression for ham stations.
- [Palomar Engineers Ferrite Toroid Calculator](https://www.palomar-engineers.com/ferrite-toroids/ferrite-toroid-design-calculator/) - Online calculator for choke impedance given core material, winding count, and frequency.
- [Fair-Rite Ferrite Products](https://www.fair-rite.com) - Primary ferrite core manufacturer; datasheets and material characteristic curves for Mix 31, 43, 61, and 75 used in ham choke construction.

### Feedline Selection and Loss

- [Times Microwave LMR Cable](https://www.timesmicrowave.com/lmr) - Industry-standard flexible coaxial cable; manufacturer's loss tables and technical specifications for LMR-400, LMR-600, and LMR-900 series.
- [The Cable Company Coax Loss Calculator](https://www.timesmicrowave.com/calculator) - Times Microwave online tool for calculating dB loss at frequency for all LMR cable types by run length.
- [DX Engineering RG-6 and Hardline Resources](https://www.dxengineering.com/search/department/coaxial-cable) - Commercial-grade feedline options including CATV hardline adaptations popular for high-power installations.
- [VK1OD Transmission Line Details](https://owenduffy.net/calc/tld.htm) - Owen Duffy's online transmission line calculator covering matched and mismatched loss, SWR, and impedance transformation.

### Antenna Modeling

- [4nec2](https://www.qsl.net/4nec2/) - Free Windows NEC2/NEC4 antenna modeling application with a visual geometry editor and far-field pattern display; the most accessible entry point for numerical antenna modeling.
- [EZNEC](https://eznec.com) - Roy Lewallen's widely used Windows antenna modeling program based on NEC2; supports up to 500 wires and is standard for most published amateur antenna designs.
- [OpenEMS](https://www.openems.de) - Open-source finite-difference time-domain (FDTD) electromagnetic field solver; handles complex structures including coax feeds, shields, and PCB antennas beyond NEC's wire-only limitations.
- [MMANA-GAL](https://hamsoft.ca/pages/mmana-gal.php) - Free antenna modeling software based on the moment method, popular for its simple interface and good accuracy for wire antennas.
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
- [fldigi](https://sourceforge.net/projects/fldigi/) - Mature multi-mode digital modem supporting PSK31, RTTY, Olivia, THOR, and dozens of others; integrates with flrig for rig control.
- [VARA HF](https://www.winlink.org/VARAHF) - High-performance adaptive HF modem used by Winlink and JS8Call; significantly outperforms older PACTOR modems at comparable price.
- [Winlink](https://www.winlink.org) - Email-over-radio network supporting HF, VHF, and satellite links; widely used for emergency communications and DX email.
- [JTDX](https://jtdx.tech) - Fork of WSJT-X with enhanced weak signal decoding algorithms; popular for difficult DX paths.
- [GridTracker](https://gridtracker.org) - Real-time map overlay for WSJT-X showing decoded callsigns, grid squares, and propagation paths.

---

## GitHub Projects

- [Hamlib](https://github.com/Hamlib/Hamlib) - The standard open-source library for rig and rotator control; supports hundreds of radios via a unified API used by nearly every ham automation tool.
- [flrig](https://github.com/w1hkj/flrig) - Rig control front-end from the fldigi suite; lightweight, cross-platform, and paired tightly with fldigi for digital mode use.
- [SDRangel](https://github.com/f4exb/sdrangel) - Full-featured SDR transceiver application with Flex SmartSDR protocol support and an extensive signal processing plugin ecosystem.
- [SoapySDR](https://github.com/pothosware/SoapySDR) - Hardware abstraction layer enabling SDR software to support many different hardware backends through a common API.
- [OpenEMS](https://github.com/thliebig/openEMS) - FDTD electromagnetic field solver for antenna and RF structure simulation beyond NEC's wire-antenna scope.
- [pyhamtools](https://github.com/dh1tw/pyhamtools) - Python library for callsign lookup, log analysis, grid square calculations, and other common ham radio data operations.
- [ham2mon](https://github.com/madengr/ham2mon) - SDR-based multi-channel scanner and recorder for monitoring amateur and public safety bands.

---

## Logging and Contesting

- [N1MM+ Logger](https://n1mmwp.hamdocs.com/) - The most widely used Windows contest logging application; supports SO2R, deep CAT integration, and band-data relay for amplifier and antenna automation.
- [Logger32](https://www.logger32.net) - Feature-rich DX logging application with multi-rig CAT control, DX cluster integration, and relay-based antenna switching outputs.
- [DXLab Suite](https://www.dxlabsuite.com) - Integrated suite of Windows applications covering logging, propagation, DX spotting, rig control, and antenna rotator management.
- [Log4OM](https://www.log4om.com) - Modern cross-platform amateur radio logging application with built-in DX cluster, LOTW/eQSL integration, and CAT rig control.
- [LOTW (Logbook of the World)](https://lotw.arrl.org) - ARRL's electronic QSL and award confirmation system; the standard for DXCC, WAS, and most major award tracking.
- [ClubLog](https://clublog.org) - Web-based log upload and analysis platform with OQRS (online QSL request), DX expedition log search, and propagation statistics.
- [eQSL](https://eqsl.cc) - Electronic QSL card exchange network accepted for some awards programs; an alternative to paper QSLs with fast confirmations.
- [N1MM Logger Plus Group](https://groups.io/g/N1MMLoggerPlus) - Official discussion and support group for N1MM Logger Plus contest logging software.
- [Logger32 Group](https://groups.io/g/hamlogger) - Community support and discussion group for Logger32 freeware logging software.

---

## Licensing and Learning

- [HamStudy](https://hamstudy.org) - Free online question pool study tool for Technician, General, and Amateur Extra exams with spaced-repetition flashcard mode.
- [ARRL](https://www.arrl.org) - The American Radio Relay League; publishes the FCC question pools, exam prep books, and the ARRL Handbook — the field's primary technical reference.
- [FCC ULS (Universal Licensing System)](https://wireless.fcc.gov/uls/) - Official FCC database for license lookup, renewal, and application; required stop for all US amateur operators.
- [Fast Track Ham Radio (AF7KB)](https://fasttrackham.com) - Michael Burnette's license preparation series covering Technician, General, and Extra class with coordinated books, audio, video, and practice exams.
- [Gordon West Training](https://gordonwestradioschool.com) - Audio and book study materials for all license classes, widely recommended for structured exam preparation.
- [Ham Radio Prep](https://hamradioprep.com) - Modern online course platform with video instruction and practice exams for all three US license classes.
- [QRZ.com](https://www.qrz.com) - Callsign lookup database, logbook, forums, and a comprehensive learning center with license exam practice tests.
