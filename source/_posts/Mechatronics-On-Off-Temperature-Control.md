---
title: Mechatronics - On/Off Temperature Control
tags:
  - Mechatronics
  - Microcontroller
  - sensor
cover: false
date: 2011-08-31 06:05:00
---

### Mechatronics - On/Off Temperature Control

One of case studies at Mechatronics class at Columbia University taught by Dr. Fred R. Stolfi.  This case study is a dynamic system investigation of an important and a common mechatronic system: a thermal close-loop system.  

The main apparatus includes:

- A microcontroller, PIC 16F74 
- A resistive heater (SRMU 100202P)
- Two temperature sensor (AD590 and AD22100)
- A fan.  


The film of On/Off temperature control:

{% youtube XYpc8UqUNBY %}


The specification of resistive heater:

| **Specifications** | **Value**             |
| ------------------ | --------------------- |
| Manufacturer       | Omega Engineering Inc |
| Model Number       | SRMU 100202P          |
| Heater Resistance  | 350 ohms              |
| Heater Area        | 4 in2                 |
| Heater Thickness   | 0.1 in                |



The specification of temperature sensor are listed below:



| **Specification**       | **AD590**    | **AD22100** |
| ----------------------- | ------------ | ----------- |
| Rated Temperature Range | -55℃ to 150℃ | 0℃ to 100℃  |
| Nominal Output at 0℃    | 273.2 μA     | 1.126 V     |
| Nominal Output at 25 0℃ | 298.2 μA     | 1.587 V     |
| Temperature Coefficient | 1μA / ℃      | 18.43 mV/℃  |
| Absolute Error          | ± 5.5 ℃      | ± 2.0 ℃     |
| Nonlinearity            | 0.8 ℃        | 0.5 ℃       |

The essential difference is that AD590 (plate) produce a current proportional to temperature while AD22100 (ambient) produce a voltage proportional to temperature. 

<!-- more -->
