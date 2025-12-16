# R-2R-4-Bit-Ladder-DAC

This repository contains the design and implementation of a **4-bit R-2R Ladder Digital-to-Analog Converter (DAC)**.  
The project demonstrates how a binary digital input can be converted into a proportional analog voltage using only two resistor values.

---

## Overview

An **R-2R ladder DAC** uses a repeating pattern of resistors with values **R** and **2R** to generate an analog output voltage corresponding to a digital input code.

This project implements a **4-bit DAC**, capable of producing **16 discrete analog output levels**.

---

## Features

- 4-bit digital input (D3–D0)
- Uses only two resistor values (R and 2R)
- Simple and cost-effective DAC design
- Suitable for learning basic DAC concepts

---

## Working Principle

- Each digital bit controls a switch connected to either **Vref (logic 1)** or **GND (logic 0)**.
- The R-2R ladder network produces weighted contributions from each bit.
- The combined output generates an analog voltage proportional to the binary input.

### Ideal Output Equation

\[
V_{out} = V_{ref} \times \left( \frac{D_3}{2} + \frac{D_2}{4} + \frac{D_1}{8} + \frac{D_0}{16} \right)
\]

where  
`D3 D2 D1 D0` ∈ {0,1}

---

## Components Used

| Component    |   Description            |
|--------------|--------------------------|
| Resistors    |   R and 2R               |
| Switches     | SPDT / logic inputs      |
| Op-amp       | (Optional) Output buffer |
| Power Supply | Reference voltage (Vref) |

---

## Testing

| Digital Input | Expected Output    |
|--------------|---------------------|
| 0000         | 0 V                 |
| 1000         | ≈ Vref / 2          |
| 1111         | ≈ Vref (full scale) |

Test the output using a **multimeter**

---


---

## Applications

- Digital-to-analog conversion basics
- Audio signal generation
- Embedded systems learning
- Electronics laboratory experiments

---

## License

This project is open-source and available under the **MIT License**.

---

## Author

**Aditi Sarkar**  
Electronics & Telecommunication Engineering  

---

*If you find this project helpful, consider giving it a star!*
