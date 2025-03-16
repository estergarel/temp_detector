# Temperature Detector

This project implements a temperature detector based on an LM35 sensor, an LM358 operational amplifier, and an LED signaling circuit. It includes both the electrical schematic and PCB design, created using OrCAD.

## Main Features

- **Temperature Sensor:** LM35, with an analog output proportional to the temperature.
- **Signal Comparison:** LM358 operational amplifier compares the detected temperature with a set threshold.
- **Visual Indication:** A red LED lights up when the temperature is below the threshold, and a green LED lights up when it exceeds the threshold.

## Components Used

| Component | Value/Model |
|------------|-------------|
| Temperature Sensor | LM35 |
| Operational Amplifier | LM358 |
| Potentiometer | 10kΩ |
| Resistors | 470Ω |
| Capacitor | 100µF |
| LEDs | Red, Green |
| Connector | 2-pin |

## Design Principles

- **Modularity:** The circuit is clearly structured into individual components for detection, comparison, and signaling.
- **Verifiable Design:** Design Rule Check (DRC) was performed, and connections were verified using Cross Reference and Wirelist.
- **PCB Optimization:** Trace widths are adjusted according to the required current (0.4mm for signals, 1mm for power lines).

## Usage Instructions

1. **Power Supply:** Connect the LM35 sensor and the rest of the circuit to a 5V power source.
2. **Threshold Adjustment:** Use the potentiometer to set the reference temperature.
3. **LED Observation:** If the detected temperature is below the threshold, the red LED stays on; if it exceeds the threshold, the green LED turns on.

## Documentation: `documentation_tie.pdf`
