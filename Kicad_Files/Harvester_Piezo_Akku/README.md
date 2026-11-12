# SiSmaK Piezoelectric Energy Harvesting Module – Battery

Custom-designed piezoelectric energy harvesting module for **[SiSmaK](https://www.spp2305.de/sismak/)** (sensor-integrating machine elements). The compact circular PCB is designed to connect to the existing SiSmaK electronics via a **flexible printed circuit (FPC)**, providing an energy harvesting interface for battery-based power supply.

The project covers schematic design, component selection, piezoelectric AC-DC rectification, power management circuitry, and PCB layout for integration into the limited installation space of the sensor-integrating bolt.

## Hardware Features

- **Energy Harvesting IC:** e-peas AEM30300
- **Energy Source:** External piezoelectric transducer
- **Rectification:** Greinacher voltage doubler using Schottky diodes and capacitors
- **Energy Harvesting:** Piezoelectric energy conversion and power management
- **Energy Storage:** Battery-based energy storage architecture
- **Power Management:** Inductive DC-DC conversion with configurable operating parameters
- **Piezoelectric Input:** External piezoelectric transducer connection via MHF4 connector
- **System Interface:** FPC connection to the existing SiSmaK electronics
- **Form Factor:** Compact circular PCB for space-constrained integration

### Piezoelectric Energy Harvesting

The module converts the alternating electrical output of an external piezoelectric transducer into usable DC energy.

A **Greinacher voltage doubler** consisting of Schottky diodes and capacitors rectifies the piezoelectric signal before it is supplied to the AEM30300 energy harvesting IC.

The AEM30300 manages the harvested energy through its integrated power management circuitry and an external inductor.

The module is designed for a battery-based energy harvesting architecture, allowing harvested energy to be stored and subsequently used to supply the SiSmaK electronics.

### SiSmaK Integration

The module was designed as an add-on to the existing SiSmaK electronics rather than a standalone development board.

The piezoelectric transducer is connected through a dedicated input connector, while the FPC interface provides the electrical connection to the sensor-integrating bolt system.

## PCB Design

The PCB was designed using **KiCad 9**, including schematic capture, component placement, and PCB routing.

### PCB View

<p align="center">
  <img src="images/Harvester_Piezo_Akku.png" width="600" alt="KiCad 3D render of the SiSmaK piezoelectric energy harvesting module">
</p>

## Hardware Design Documentation

The KiCad schematic and PCB design files are included for further inspection.

[View Hardware Design Documentation (PDF)](Hardware_Design.pdf)

## Design Files

| File | Description |
|---|---|
| `Harvester_Piezo_Akku.kicad_pro` | KiCad project |
| `Harvester_Piezo_Akku.kicad_sch` | Electrical schematic |
| `Harvester_Piezo_Akku.kicad_pcb` | PCB layout |
| `images/Harvester_Piezo_Akku.png` | KiCad 3D rendering |
| `Hardware_Design.pdf` | Schematic and PCB documentation |

## Project Status

PCB design documented. Manufacturing and hardware validation status are not specified here.

---

**Author:** Alexander Richter  
**Institution:** TU Darmstadt  
**Related project:** [SiSmaK – Project Website](https://www.spp2305.de/sismak/)