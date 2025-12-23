# R-2R-4-Bit-Ladder-DAC

This repository contains the design and implementation of a **4-bit R-2R Ladder Digital-to-Analog Converter (DAC) PCB**.  
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

$Vout = -\frac{R_{ref}}{R} \frac{V_{ref}}{2^4} [\frac{D_3}{2} + \frac{D_2}{4} +\frac{D_1}{8} +\frac{D_0}{16} ]  $


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





## Tools & Software

- # EasyEDA – Circuit simulation & PCB design

- # Tinkercad – Online circuit verification

----
## PCB [R-2R 4-bit Ladder DAC Using IC 741]
# PCB Dimension: length: 6 cm, height: 4.5 cm
# PCB Images:
- [PCB Front side:](https://github.com/Aditisarkar16122001/R-2R-4-Bit-Ladder-DAC/blob/main/Images/Picture5-PCB%20Top%20Side.jpg)
- [PCB Back side:](https://github.com/Aditisarkar16122001/R-2R-4-Bit-Ladder-DAC/blob/main/Images/Picture6-PCB%20Bottom%20Side.jpg)
-----

## Results
- Output voltage increases monotonically with digital input

- Practical results closely match theoretical and simulated values

- Minor deviations due to component tolerances and non-idealities

----
## Digital Input Vs Analog Output Comparison:
[Digital Input Vs Analog Output Comparison](https://github.com/Aditisarkar16122001/R-2R-4-Bit-Ladder-DAC/blob/main/ip%20vs%20op%20image.png)
## Applications

- Digital-to-analog conversion basics
- Audio signal generation
- Embedded systems learning
- Electronics laboratory experiments

---

## References
- EasyEDA

- Tinkercad

- Standard Analog Electronics textbooks
----
## Author

**Aditi Sarkar**  
Electronics & Telecommunication Engineering  

---

*If you find this project helpful, consider giving it a star!*
