# SiSmaK Solar Energy Harvesting Module – Battery

Custom-designed photovoltaic energy harvesting module for **[SiSmaK](https://www.spp2305.de/sismak/)** (sensor-integrating machine elements). The compact circular PCB is designed to connect to the existing SiSmaK electronics via a **flexible printed circuit (FPC)**, providing an energy harvesting interface for battery-based power supply.

The project covers schematic design, component selection, power management circuitry, and PCB layout for integration into the limited installation space of the sensor-integrating bolt.

## Hardware Features

- **Energy Harvesting IC:** e-peas AEM10300
- **Energy Source:** External photovoltaic cells
- **Energy Harvesting:** Photovoltaic energy conversion and power management
- **Energy Storage:** Battery-based energy storage architecture
- **Power Management:** Inductive DC-DC conversion with configurable operating parameters
- **System Interface:** FPC connection to the existing SiSmaK electronics
- **Form Factor:** Compact circular PCB for space-constrained integration

### Photovoltaic Energy Harvesting

The AEM10300 is used to harvest electrical energy from external photovoltaic cells. The circuit integrates the required passive components and configuration connections for energy harvesting and power management.

The module is designed for a battery-based energy harvesting architecture, in which harvested energy can be stored and subsequently used to supply the SiSmaK electronics.

### SiSmaK Integration

The module was designed as an add-on to the existing SiSmaK electronics rather than a standalone development board. Its FPC interface provides the electrical connection to the sensor-integrating bolt system.

## PCB Design

The PCB was designed using **KiCad 9**, including schematic capture, component placement, and PCB routing.

### PCB View

<p align="center">
  <img src="images/Harvesting_Solar_Akku.png" width="600" alt="KiCad 3D render of the SiSmaK solar energy harvesting module">
</p>

## Hardware Design Documentation

The KiCad schematic and PCB design files are included for further inspection.

[View Hardware Design Documentation (PDF)](Hardware_Design.pdf)

## Design Files

| File | Description |
|---|---|
| `Harvesting_Solar_Akku.kicad_pro` | KiCad project |
| `Harvesting_Solar_Akku.kicad_sch` | Electrical schematic |
| `Harvesting_Solar_Akku.kicad_pcb` | PCB layout |
| `images/Harvesting_Solar_Akku.png` | KiCad 3D rendering |
| `Hardware_Design.pdf` | Schematic and PCB documentation |

## Project Status

PCB design documented. Manufacturing and hardware validation status are not specified here.

---

**Author:** Alexander Richter  
**Institution:** TU Darmstadt  
**Related project:** [SiSmaK – Project Website](https://www.spp2305.de/sismak/)