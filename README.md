# Dual Laser Engraving and Pencil Plotter Machine
This project is a DIY multi-functional CNC machine capable of both pen plotting and laser engraving.

You can swap between a pen holder (for precision drawing) and a laser module (for engraving and light cutting. Thus, getting the benift of both.

<img width="903" alt="Screenshot 2025-05-30 at 10 09 55 PM" src="https://github.com/user-attachments/assets/9a09ab16-17f8-4511-96b5-0a1a03db0bdc" />

# Motivation
The aim is to develop a cost-effective and versatile CNC device that would incorporate all the characteristics of a pen plotter and a laser engraver. By modularizing the system, you will be able to quickly switch from drawing to engraving, or an array of representative and technical endeavors.

# Tools/Technology needed:
- CAD Software: Fusion 360 (Web Version)
- Firmware: Compatible with GRBL-based controllers
- Control Board: MKS DLC32
- Touchscreen: MKS TS35
- Design Software: Inkscape with plugins, LightBurn, LaserGRBL


| Component                           | Quantity | Estimated Cost (USD) | Source         |
| ----------------------------------- | -------- | -------------------- | -------------- |
| 20x20 Aluminum Extrusions           | 5        | \$25                 | Local Supplier |
| Stepper Motors (NEMA 17)            | 3        | \$30                 | Aliexpress     |
| Stepper Motor Cables                | 3        | \$5                  | Aliexpress     |
| Stepper Motor Controller Board (L1) | 1        | \$15                 | Aliexpress     |
| Timing Belts and Pulleys            | 2 sets   | \$10                 | Aliexpress     |
| Screws, Washers, Spacers            | Various  | \$10                 | Local Supplier |
| Laser Module (20W)                  | 1        | \$60                 | Aliexpress     |
| MKS DLC32 Control Board             | 1        | \$20                 | Aliexpress     |
| MKS TS35 Touchscreen                | 1        | \$25                 | Aliexpress     |
| Acrylic Panels                      | 6        | \$15                 | Local Supplier |
| Power Supply Unit                   | 1        | \$20                 | Aliexpress     |
| Miscellaneous (Wiring, Connectors)  | Various  | \$10                 | Local Supplier |

Total Estimated Cost: ~$250 Please not that the BOM is really first draft the BOM is likely to go up

# Assembly Instructions
1. 3D print the files form the repo in the /cad folder
2. Assemble the 20x20 aluminum extrusions using the aluminum corner fittings to form a sturdy rectangular frame.
3. Install the stepper motors on the frame of the x and y mechanism
4. Attach the timing belts and pulleys to the stepper motors and the moving parts of the X and Y axes.
5. Attach the 20W laser module/ pen plotter mount depending on you use cae securely onto the carriage.
6. For the pencil plotter remember to place a spring above the pen to apply downward pressure, ensuring consistent contact with the paper during plotting.
7. Mount the MKS DLC32 control board onto the frame.
8. Connect the stepper motors, laser module, and other components to the control board as per the wiring diagram. WIP
9. Install the MKS TS35 touchscreen for user interface and control.
10. Firmware and Software Setup:
- Install GRBL firmware on the MKS DLC32 control board 
- Configure the firmware settings to match the specifications of your machine. (WIP)
- Use software like Inkscape with plugins, LightBurn, or LaserGRBL to create and send G-code files to the machine.

# Power Supply (12 V, ≥6 A)
12 V PSU +  ─> VIN+ on MKS DLC32

12 V PSU –  ─> GND on  MKS DLC32

# MKS TS35 Touchscreen
TS35 VCC ─> 5 V on MKS DLC32

TS35 GND ─> GND on MKS DLC32

TS35 TX  ─> RX2 (U2RX) on   MKS DLC32

TS35 RX  ─> TX2 (U2TX) on   MKS DLC32

# Stepper Drivers (A4988) & NEMA17 Motors
A4988 VDD ─> 5 V on MKS DLC32

A4988 GND ─> GND on   MKS DLC32

A4988 VMOT ─> 12 V PSU +

A4988 GND -> 12 V PSU –  (same as MKS DLC32 GND)

A4988 STEP ─> X: STP_X on MKS DLC32  (use “X-STEP” pin)

A4988 DIR ─> X: DIR_X on MKS DLC32  (use “X-DIR” pin)

A4988 EN ─> X: EN_X on  MKS DLC32  (tie LOW or to “X-EN”)



A4988 STEP ─> Y: STP_Y on MKS DLC32  (use “Y-STEP” pin)

A4988 DIR ─> Y: DIR_Y on MKS DLC32  (use “Y-DIR” pin)

A4988 EN ─> Y: EN_Y on  MKS DLC32  (tie LOW or to “Y-EN”)

Motor coils ─> A4988 1A,1B,2A,2B (match coil pairs)

# Z-Axis Pen Lift (SG90 Servo)
SG90 Signal ─> PWM1 on MKS DLC32  

SG90 VCC ─> 5 V on MKS DLC32

SG90 GND ─> GND on   MKS DLC32


Laser PWM ->  Laser PWM Output on MKS DLC32 
Laser VCC ─> +12 V PSU +

Laser GND ─> GND (shared)

