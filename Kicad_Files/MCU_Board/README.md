# Nordic nRF54L Custom Development Board

Custom Nordic MCU development-board design for firmware prototyping, peripheral access, and debugging. The supplied schematic and PCB specify **`NRF54L15-QFAA-R`**; 

Development covered the MCU support circuit, supply filtering and decoupling, clock components, RF network, schematic capture, and PCB layout. This is a separate board design; it is not the existing flexible SiSmaK electronics.

## Hardware Features

- **Microcontroller:** Nordic nRF54L15 in the supplied Value/MPN fields
- **RF Circuit:** Discrete matching network and ACAG0201-2450-T chip antenna
- **Clocking:** External high-frequency crystal oscillator
- **Power Supply:** Direct external supply with MCU decoupling and filtering
- **Debugging:** SWD interface for programming and debugging
- **GPIO Expansion:** Pin headers providing access to MCU GPIOs and peripheral interfaces
- **User Interface:** Reset button, user button, and two status LEDs


### Debugging and Peripheral Access

SWDIO, SWDCLK, and reset connections provide programming/debug access. Pin headers expose GPIOs, including signals labelled for peripheral buses, so external circuits can be connected without modifying the PCB.

Two LEDs, a user button, and a reset button provide local controls and status outputs. These are hardware provisions; tested firmware drivers and peripheral functionality are not documented for this board.

## PCB Design

The four-layer PCB was designed using **KiCad 9**. The project includes custom design rules alongside the schematic and layout.

### PCB Layout

<p align="center">
  <img src="images/pcb_layout.png" width="800" alt="PCB Layout">
</p>

## Schematics

The existing hardware PDF export is available here:

[View Schematic (PDF)](Hardware_Design.pdf)

The original KiCad project files are also included for further inspection.

## Design Files

| File | Description |
|---|---|
| [`MCU_Board.kicad_pro`](MCU_Board.kicad_pro) | KiCad project |
| [`MCU_Board.kicad_sch`](MCU_Board.kicad_sch) | Main schematic |
| [`MCU.kicad_sch`](MCU.kicad_sch) | MCU schematic sheet |
| [`MCU_Board.kicad_pcb`](MCU_Board.kicad_pcb) | PCB layout |
| [`MCU_Board.kicad_dru`](MCU_Board.kicad_dru) | Custom design rules |



---

**Author:** Alexander Richter  
**Institution:** TU Darmstadt
