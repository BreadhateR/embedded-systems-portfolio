# Embedded Systems & PCB Design Portfolio

Hardware designs and experimental work from my master's thesis on the power supply of **[SiSmaK – Sensor-integrated machine element](https://www.spp2305.de/sismak/)** at TU Darmstadt. SiSmaK is a sensor-integrated M20 bolt that measures multiaxial mechanical loads using strain gauges and transmits the readings wirelessly. The thesis investigated photovoltaic harvesting, externally driven ultrasonic power transfer, and NFC power transfer as alternative supplies for the existing sensor electronics.

My work covered power-supply concepts, component selection, schematic and PCB design, analog measurement circuits, firmware adaptations, system integration, and experimental characterization. The main challenges were the approximately **13 mm PCB diameter**, limited storage capacity, and MCU startup and measurement bursts that exceed the available harvesting power. Each project README explains its circuit, design decisions, and validation scope alongside the KiCad files and existing hardware PDF.

## Projects

| Project | Focus | Documentation |
| --- | --- | --- |
| **[MCU Board](Kicad_Files/MCU_Board/)** | Separate Nordic MCU development-board design with RF, SWD and GPIO interfaces | [README](Kicad_Files/MCU_Board/README.md) · [Hardware design](Kicad_Files/MCU_Board/Hardware_Design.pdf) |
| **[Solar Harvester — Battery](Kicad_Files/Harvesting_Solar_Akku/)** | AEM10300 photovoltaic supply using the existing SiSmaK rechargeable cell | [README](Kicad_Files/Harvesting_Solar_Akku/README.md) · [Hardware design](Kicad_Files/Harvesting_Solar_Akku/Hardware_Design.pdf) |
| **[Solar Harvester — Capacitor](Kicad_Files/Harvester_Solar_Kondensator/)** | Photovoltaic supply with 150 µF storage and a storage-controlled output gate | [README](Kicad_Files/Harvester_Solar_Kondensator/README.md) · [Hardware design](Kicad_Files/Harvester_Solar_Kondensator/Hardware_Design.pdf) |
| **[Piezo Harvester — Battery](Kicad_Files/Harvester_Piezo_Akku/)** | Ultrasonic receiver supply with Greinacher rectification and AEM30300 load adjustment | [README](Kicad_Files/Harvester_Piezo_Akku/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_Akku/Hardware_Design.pdf) |
| **[Piezo Harvester — Capacitor](Kicad_Files/Harvester_Piezo_Kondensator/)** | Ultrasonic supply architecture with capacitor storage and phased measurement operation | [README](Kicad_Files/Harvester_Piezo_Kondensator/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_Kondensator/Hardware_Design.pdf) |
| **[Piezo Harvester with Measurements](Kicad_Files/Harvester_Piezo_WithMeasurements/)** | Compact rectifier-output voltage/current measurement design for frequency ranking | [README](Kicad_Files/Harvester_Piezo_WithMeasurements/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_WithMeasurements/Hardware_Design.pdf) |
| **[Piezo Harvesting & Resonance Evaluation Board](Kicad_Files/Harvester_Piezo_WithMeasurements__DevBoard/)** | Configurable harvesting and measurement platform with XIAO nRF54L15 and SiSmaK interfaces | [README](Kicad_Files/Harvester_Piezo_WithMeasurements__DevBoard/README.md) · [Hardware design](Kicad_Files/Harvester_Piezo_WithMeasurements__DevBoard/Hardware_Design.pdf) |
| **[NFC Harvester](Kicad_Files/NFC_Harvester/)** | NTAG 5 Link receiver with antenna tuning and reverse-current blocking | [README](Kicad_Files/NFC_Harvester/README.md) · [Hardware design](Kicad_Files/NFC_Harvester/Hardware_Design.pdf) |


## Repository Structure

```text
Kicad_Files/
├── MCU_Board/
├── Harvesting_Solar_Akku/
├── Harvester_Solar_Kondensator/
├── Harvester_Piezo_Akku/
├── Harvester_Piezo_Kondensator/
├── Harvester_Piezo_WithMeasurements/
├── Harvester_Piezo_WithMeasurements__DevBoard/
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

The existing SiSmaK sensor electronics, flexible PCB, and overall bolt concept formed the integration baseline. The harvesting modules and associated firmware/measurement work documented here extend that system; they do not represent development of the complete SiSmaK platform. 


The experiments demonstrated solar-powered measurement and wireless transmission under sufficiently strong artificial illumination, phased operation with a **150 µF capacitor**, and about **40 mW maximum NFC output at 1 cm coil spacing** in the tested aluminium-bolt setup. The project pages state the relevant conditions and limitations. Circuit development used **KiCad 9** and **LTspice**; validation used SMU load sweeps, **Nordic PPK2**, an oscilloscope, and **NanoVNA** impedance measurements. Firmware and host-program behavior are described in the thesis; their source code is not included in this repository.
