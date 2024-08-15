# Intro
A pcb with a single button, which on each press toggles a mosfet's output on/off, acting like a mechanical switch. 

# Specs

- Current troughput theoretically: around 10A
- PCB input voltage: 3.0V - 5.0V
- Thicc exposed mosfet traces to create solder wires

# Properties

- Initial state is off
- Two n-channel mosfets in parallel for high current support
- Green status led (optional)
- Debounced button

# Usage

- Connect e.g. a li-ion battery's GND to the pcb's GND
- Connect li-ion VCC to pcb's VCC
- Connect li-ion VCC to e.g. a motor's VCC
- Connect pcb's DR to motor's GND

## PCB

<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/6b391ccb-ca41-4e43-80a1-11a88502983b" alt="PCB Top View"/>
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/515bbead-8dd3-4e98-9a89-3779f90523d0" alt="PCB Bottom View"/>
    </td>
  </tr>
</table>
