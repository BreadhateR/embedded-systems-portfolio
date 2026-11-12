# SiSmaK NFC Energy Harvesting Module

Custom-designed NFC energy harvesting module for **[SiSmaK](https://www.spp2305.de/sismak/)** (sensor-integrating machine elements). The compact circular PCB is designed to connect to the existing SiSmaK electronics via a **flexible printed circuit (FPC)**, providing an interface for NFC-based energy transfer.

The project covers schematic design, component selection, antenna tuning circuitry, and PCB layout for integration into the limited installation space of the sensor-integrating bolt.

## Hardware Features

- **NFC IC:** NXP NTAG 5 Link (NTP5332)
- **Energy Harvesting:** NFC field energy converted to a DC output
- **Antenna Interface:** External antenna via MHF4 connector with tuning capacitors
- **Power Path:** LM66100 ideal-diode controller for output power-path control
- **System Interface:** FPC connection to the existing SiSmaK electronics, exposing power and control/data signals
- **Form Factor:** Compact circular PCB for space-constrained integration

### NFC Energy Harvesting

The NTAG 5 Link provides an NFC interface with energy harvesting capability. An antenna matching/tuning network connects the external NFC antenna to the IC, while the harvested voltage is routed through the output power path.

### SiSmaK Integration

The module was designed as an add-on to the existing SiSmaK electronics rather than a standalone development board. Its FPC interface provides the electrical connection to the sensor-integrating bolt system.

## PCB Design

The PCB was designed using **KiCad 9**, including schematic capture, component placement, and PCB routing.

### PCB View

<p align="center">
  <img src="images/NFC_Harvester.png" width="600" alt="KiCad 3D render of the SiSmaK NFC energy harvesting module">
</p>

## Schematics

## Hardware Design Documentation

The KiCad schematic and PCB design files are included for further inspection.

[View Hardware Design Documentation (PDF)](Hardware_Design.pdf)

## Design Files

| File | Description |
|---|---|
| `NFC_Harvester.kicad_pro` | KiCad project |
| `NFC_Harvester.kicad_sch` | Electrical schematic |
| `NFC_Harvester.kicad_pcb` | PCB layout |
| `images/NFC_Harvester.png` | KiCad 3D rendering |

## Project Status

PCB design documented. Manufacturing and hardware validation status are not specified here.

---

**Author:** Alexander Richter  
**Institution:** TU Darmstadt  
**Related project:** [SiSmaK – Project Website](https://www.spp2305.de/sismak/)
