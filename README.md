# Intro

A pcb with a single button, which on each press toggles a mosfet's output on/off, acting like a mechanical switch. 

## PCB

<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/6b391ccb-ca41-4e43-80a1-11a88502983b" alt="PCB Top View"/>
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/515bbead-8dd3-4e98-9a89-3779f90523d0" alt="PCB Bottom View"/>
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/6b391ccb-ca41-4e43-80a1-11a88502983b" alt="PCB Top View"/>
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/6b391ccb-ca41-4e43-80a1-11a88502983b" alt="PCB Top View"/>
    </td>
  </tr>
</table>

## Specs

- Current troughput theoretically: around 10A
- PCB input voltage: 3.0V - 5.0V
- Thicc exposed mosfet traces to create solder wires

## Properties

- Power consumption
  - Switched off:
    - 0.0 uA @ 2.5 V (= less than 100 nA)
    - 4 uA @ 4.2 V
    - 25 uA @ 5.0 V
  - Switched on:
    - 240 uA @ 2.5V
    - 500 uA @ 4.2V
    - 500 uA @ 5.0 V
- Initial state is off
- Two n-channel mosfets in parallel for high current support
- Green status led (optional)
- Debounced button

## BOM
R1: 0805 sized, 10k
R2: 0805 sized, 10k
R3: 0805 sized, 10k
C1: 0805 sized, 100nF
C2: 0805 sized, 100nF
U1: SOP16 package, CD4013BM
U2: sot23-3 package, AO3400
U3: sot23-3 package, AO3400
S1: Tactile switch CK (Metal shell)
D1: 3528 sized, RGB led with common VCC

## Usage

- Connect e.g. a li-ion battery's GND to the pcb's GND
- Connect li-ion VCC to pcb's VCC
- Connect li-ion VCC to e.g. a motor's VCC
- Connect pcb's DR to motor's GND


## Schematic

![image](https://github.com/user-attachments/assets/6a2cfb31-8441-47f3-87af-41b553e52850)
