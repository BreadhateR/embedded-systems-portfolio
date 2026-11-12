# Embedded Systems & PCB Design Portfolio

A collection of KiCad hardware designs developed as part of work on **[SiSmaK – Sensor-integrated machine element](https://www.spp2305.de/sismak/)** at TU Darmstadt.

The projects focus on compact, low-power embedded hardware, energy harvesting, sensor interfaces, and electrical measurements. Each project folder contains its KiCad design files, a dedicated README, and a PDF export of the hardware documentation.

## Projects

| Project | Focus | Documentation |
| --- | --- | --- |
| **[MCU Board](Kicad_Files/MCU_Board/)** | Compact embedded controller PCB and supporting circuitry | [README](Kicad_Files/MCU_Board/README.md) · [Hardware design](Kicad_Files/MCU_Board/Hardware_Design.pdf) |
| **[Solar Harvester — Battery](Kicad_Files/Harvesting_Solar_Akku/)** | Photovoltaic energy harvesting with rechargeable energy storage | [README](Kicad_Files/Harvesting_Solar_Akku/README.md) · [Hardware design](Kicad_Files/Harvesting_Solar_Akku/Hardware_Design.pdf) |
| **[Solar Harvester — Capacitor](Kicad_Files/Harvester_Solar_Kondensator/)** | Photovoltaic harvesting with capacitive storage | [README](Kicad_Files/Harvester_Solar_Kondensator/README.md) · [Hardware design](Kicad_Files/Harvester_Solar_Kondensator/Hardware_Design.pdf) |
| **[Piezo Harvester — Battery](Kicad_Files/Harvester_Piezo_Akku/)** | Piezoelectric harvesting with battery storage | [README](Kicad_Files/Harvester_Piezo_Akku/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_Akku/Hardware_Design.pdf) |
| **[Piezo Harvester — Capacitor](Kicad_Files/Harvester_Piezo_Kondensator/)** | Piezoelectric harvesting with capacitive storage | [README](Kicad_Files/Harvester_Piezo_Kondensator/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_Kondensator/Hardware_Design.pdf) |
| **[Piezo Harvester with Measurements](Kicad_Files/Harvester_Piezo_WithMeasurments/)** | Integrated piezoelectric harvesting and voltage/current measurement circuits for resonance search | [README](Kicad_Files/Harvester_Piezo_WithMeasurments/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_WithMeasurments/Hardware_Design.pdf) |
| **[Piezo Harvesting & Resonance Evaluation Board](Kicad_Files/Harvester_Piezo_WithMeasurments__DevBoard/)** | Development platform for evaluating harvesting and resonance-search measurements | [README](Kicad_Files/Harvester_Piezo_WithMeasurments__DevBoard/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_WithMeasurments__DevBoard/Hardware_Design.pdf) |
| **[NFC Harvester](Kicad_Files/NFC_Harvester/)** | NFC-based energy harvesting | [README](Kicad_Files/NFC_Harvester/README.md) · [Hardware design](Kicad_Files/NFC_Harvester/Hardware_Design.pdf) |


## Repository Structure

```text
Kicad_Files/
├── MCU_Board/
├── Harvesting_Solar_Akku/
├── Harvester_Solar_Kondensator/
├── Harvester_Piezo_Akku/
├── Harvester_Piezo_Kondensator/
├── Harvester_Piezo_WithMeasurments/
├── Harvester_Piezo_WithMeasurments__DevBoard/
├── NFC_Harvester/
└── Libraries/
    ├── 3D/
    ├── Footprints/
    └── Symbols/
```

Project directories generally include:

- `*.kicad_pro`, `*.kicad_sch`, `*.kicad_pcb` — editable KiCad project, schematic, and PCB layout
- `README.md` — project-specific description
- `Hardware_Design.pdf` — exported hardware documentation
- `images/` — board renders or layout images
- `bom/` — bill-of-materials exports where available, including interactive BOMs

Shared custom symbols, footprints, and 3D models are located in [`Kicad_Files/Libraries/`](Kicad_Files/Libraries/).

## Viewing the Designs

Open a project's `.kicad_pro` file in **KiCad** to inspect its schematic and PCB layout. For a quick overview without KiCad, use the project's README, PDF documentation, and available interactive BOM (`bom/ibom.html`).


## Project Context

These designs were developed in the context of the **[SiSmaK project](https://www.spp2305.de/sismak/)** at **TU Darmstadt**. It is not a complete reproduction of the overall SiSmaK system.
