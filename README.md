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
