# Laser-Engraving-Machine
This project is a DIY multi-functional CNC machine capable of both pen plotting and laser engraving.

You can swap between a pen holder (for precision drawing) and a laser module (for engraving and light cutting. Thus, getting the benift of both.

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

Total Estimated Cost: ~$285 Please not that the BOM is really first draft

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


