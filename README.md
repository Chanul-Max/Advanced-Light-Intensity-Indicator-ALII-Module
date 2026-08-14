# 💡 Advanced Light Intensity Indicator (ALII) Module

Welcome to the documentation for the Advanced Light Intensity Indicator (ALII) module! This project was developed as a Semester 03 Digital Signal Processing assignment with a rigorous constraint: **No programmable ICs allowed.** 

By bridging analog and digital engineering fundamentals, our team designed a smart, sustainable system from scratch to solve real-world problems using purely hardware-based logic.

## 🛠️ Tech Stack & Hardware Components
Wiring this complex architecture on a breadboard was a massive challenge that tested our patience and creativity. Seeing the system come to life without a single line of code made every late night worth it.

*   **Logic Processing:** 74LS Family Logic Gates
*   **Signal Conditioning:** Operational Amplifiers (Op-Amps)
*   **Timing & Pulses:** NE555 Timers

## ✨ System Architecture & Achievements

*   **A "Clean" Signal:** We designed a custom analog filter to effectively wipe out power line noise, ensuring that the raw data feeding into the system remained stable and accurate.
*   **The "Watchdog" Stability:** Instead of relying on simple delays, we engineered an adjustable logic circuit (30–300s) that acts as a watchdog, successfully preventing false triggering caused by sudden, transient light fluctuations in the environment.
*   **The 15-Minute Average (Voltage-to-Frequency):** Since we couldn't code a math function into a microcontroller, we utilized a Voltage-to-Frequency conversion technique. By converting light intensity into pulses using NE555 Timers, we counted them over 300–900 seconds to find the true average. This required precise mathematical modeling of the timer circuitry—specifically ensuring the $T_{low}$ value was strictly accounted for and exact resistor coefficients were applied (omitting the common erroneous multiplier of 2 in front of the $R_2$ variable in standard timing equations) to guarantee highly accurate pulse counting.

## 🤝 The Team
A massive shoutout to my group members for their dedication, imagination, and brilliant engineering throughout this project:
*   Achintha Niroshan
*   Danul Renuja
*   Prathibha Nirukthi
*   Yasiru Pamod

---
*Proudly built at the University of Moratuwa (#UoM) | #ElectricalEngineering #DigitalSignalProcessing #HardwareDesign #NoCode*
