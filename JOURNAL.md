Made by: @codelife / @programmer6
# Dual CNC machine - pen plotting and laser engraving.

**Project Status:** Waiting-Review

**Total Design Hours:** 

**CAD:** https:/a360.co/4jtUqSq

**Respository link:**  https://github.com/Programer6/Laser-Engraving-Machine

**BOM:** 


## Project Overview
This project is a DIY multi-functional CNC machine capable of both pen plotting and laser engraving.

You can swap between a pen holder (for precision drawing) and a laser module (for engraving and light cutting. Thus, getting the benift of both.

## Research: 2 Hour - 20th May 2025

Spent about two hours researching how laser engravers and pen holders actually work. Brain dump of what learn/ reseached:
-  Stepper motors and belts or screws to control the X and Y axes
-  Running special firmware that interprets G-code 
-  Instructions that tell the machine exactly where to move and when to turn the laser on or lift the pen.
-  pen holder -you need a mechanism to raise and lower the pen so it only touches the paper when it’s supposed to draw
-  This will need ot be able to easily swapped with a laser engraver, a laser diode is mounted instead of the pen
-  Learned a bit about programes such as  Inkscape with plugins, LightBurn, or LaserGRBL


# 4-5 Hour - 20th May 2025

Today i spent crazy amount of time designing the linear rail profile in which I had to make carfull consideration of the alignment and spacing - Sketch and extrude to fit 2020 extrusions. This is the end result from the work: I hade to make one and then mirror the other 
<img width="543" alt="Screenshot 2025-05-30 at 8 30 52 PM" src="https://github.com/user-attachments/assets/02e9683d-df95-49eb-9bbf-1de11932c8c3" />
<img width="220" alt="Screenshot 2025-05-30 at 8 32 50 PM" src="https://github.com/user-attachments/assets/9e33ff5b-9bf2-4c64-bde8-eee25e3592e2" />
<img width="358" alt="Screenshot 2025-05-30 at 9 00 37 PM" src="https://github.com/user-attachments/assets/9d4a6edc-c390-4353-8c1c-02e67397262e" />
<img width="271" alt="Screenshot 2025-05-30 at 9 01 10 PM" src="https://github.com/user-attachments/assets/b7963f76-e5e5-4674-b4c1-36ade7ab0397" />


# 1-2 Hour - 28th May 2025
Today, I finished by creating the rolling tool head mechanism as you can see in the image. This goal of this was to make make it easily swappably between the laser diode and well as the pencil plotter.
<img width="686" alt="Screenshot 2025-05-30 at 8 35 21 PM" src="https://github.com/user-attachments/assets/89ef7d8b-ebdd-43e2-ba39-05967cf3a9b7" />
<img width="567" alt="Screenshot 2025-05-30 at 9 01 44 PM" src="https://github.com/user-attachments/assets/ae9f60a5-1353-4592-ac39-879a013da294" />
<img width="533" alt="Screenshot 2025-05-30 at 9 01 58 PM" src="https://github.com/user-attachments/assets/5ef63c31-9f25-4dec-b17f-493dd7d9bdfa" />
<img width="657" alt="Screenshot 2025-05-30 at 9 02 16 PM" src="https://github.com/user-attachments/assets/a1dd89e8-65d0-416e-bbc6-744a5129281f" />


# 3 Hour - 29th May 2025
Inorder for all the 4 extrusion to hold up and create the sqare sturcture I needed to create a frame corners cad module and cosidering that i had the most cytrical components out of the way I also focused on assembling the the laser engraver together thus by the end of this day I was truly able to bring the machine into life. On a side note, Fusion360 crashed & like hangged multiple times so  tired out the Web verison which made it some much easier as all of the processing happened in the servers.

<img width="158" alt="Screenshot 2025-05-30 at 8 42 19 PM" src="https://github.com/user-attachments/assets/a3430e79-7dbb-4a8c-b2cd-21bfccfaacc0" />
<img width="238" alt="Screenshot 2025-05-30 at 8 48 03 PM" src="https://github.com/user-attachments/assets/c4589ba1-7639-4812-801c-4384eeb03c68" />
<img width="749" alt="Screenshot 2025-05-30 at 9 05 33 PM" src="https://github.com/user-attachments/assets/60d07cd1-bfe6-439c-88e7-a7eb1e746f90" />


# 3 Hour - 29th May 2025
Added the final touches and design tochscreen holder for MKS TS35 and MKS DLC32 board case attached to the 20*20 extrusions

<img width="781" alt="Screenshot 2025-05-30 at 8 51 41 PM" src="https://github.com/user-attachments/assets/c93cc841-5e6a-4f6b-8080-2665a99b9a21" />
<img width="474" alt="Screenshot 2025-05-30 at 9 04 24 PM" src="https://github.com/user-attachments/assets/f552fbc6-718f-4ccc-8082-f69657153370" />


# Final Design without toolhead:
<img width="943" alt="Screenshot 2025-05-30 at 8 59 40 PM" src="https://github.com/user-attachments/assets/c37eab13-675c-4d67-b6bc-135fe4859ab3" />


#So for the toolhead: 

For the laser engraver I am using the module made by MELKANO as it really well desinged with no need for modification while I custom designed my pencil plotter using a mecahnism in which the pen is mounted inside a pen holder tube or carriage. The pen can move up and down freely inside this tube with a spring is placed above which pushes the pen downward so that when the pen is lowered onto the paper, it makes contact lightly but firmly.

<img width="411" alt="Screenshot 2025-05-30 at 9 06 48 PM" src="https://github.com/user-attachments/assets/f6ae0b6c-744c-4e44-9080-2a4ec37db868" />
