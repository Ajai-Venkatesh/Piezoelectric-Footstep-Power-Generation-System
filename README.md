# Piezoelectric-Footstep-Power-Generation-System
Energy harvesting system using piezoelectric discs with Arduino-based voltage monitoring
⚡ Project Title

Piezoelectric Footstep Power Generation System with Arduino Monitoring

📖 Overview

This project is a renewable energy harvesting system that converts mechanical energy from human footsteps into electrical energy using piezoelectric discs. The generated energy is rectified, stored in a battery, and monitored using an Arduino-based system.

🎯 Objectives
Harvest energy from footsteps
Convert AC → DC using rectifier
Store energy in battery/supercapacitor
Monitor voltage using Arduino
Demonstrate smart flooring concept
⚙️ Working Principle

Footstep pressure → Piezoelectric discs generate AC voltage → Bridge rectifier converts to DC → Filter capacitor smooths output → Battery stores energy → Arduino monitors voltage via voltage divider.
🔧 Components Used
Piezoelectric discs
1N4007 diodes (Bridge Rectifier)
Capacitor (Filter)
Battery (Li-ion / 12V)
DC-DC converter (optional)
Arduino UNO
Voltage divider resistors
LCD display (optional)

flowchart TD
    A[Footstep Pressure] --> B[Piezoelectric Discs Array]

    B --> C[Bridge Rectifier<br>1N4007 Diodes]
    C --> D[Filter Capacitor<br>100uF - 1000uF]
    D --> E[Battery Storage<br>3.7V / 12V]

    E --> F[DC Load / Inverter]

    E --> G[Voltage Divider<br>R1=100kΩ R2=10kΩ]
    G --> H[Arduino UNO<br>Analog Pin A0]
    H --> I[LCD Display / Serial Monitor]

    style A fill:#e3f2fd,stroke:#333
    style B fill:#bbdefb,stroke:#333
    style C fill:#ffe0b2,stroke:#333
    style D fill:#ffe0b2,stroke:#333
    style E fill:#c8e6c9,stroke:#333
    style F fill:#ffcdd2,stroke:#333
    style G fill:#d1c4e9,stroke:#333
    style H fill:#d1c4e9,stroke:#333
    style I fill:#d1c4e9,stroke:#333
