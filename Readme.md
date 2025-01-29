# UV TIMER
Your friendly neighbourhood timer.

### About the project
This project is a hardware timer based on Arduino.

It uses the Arduino Nano as the controller and WE___  16*2 display and push buttons to interface with the user. 

The UV is driven by IRFZ44N mosfet and two L7805CV regulators are placed in parallel to help provide current for heavy loads.

The UV Timer can be powered by a 12V or 5V adapter. 

A jumper is provided that can be used to set the voltage for the load (5V or 12V).

>*Project PIC HERE*


## HARDWARE
## PCB

### Schematic and PCB design
The schematic and PCB for this project was designed using $"Kicad".

->Schematic "/././.sch"

>*INSERT SCHEMATIC PIC HERE*

-> PCB "/././.pcb"
>*INSERT PCB PIC HERE*

### PCB Fabrication
Fabrication of the PCB for this project was done in-house at @Robotics Club,Pulchowk. 
    
The fabrication method and guide used can be found *#here#* 

> PDB FRONT PIC

> PCB BACK PIC

### Bill Of Materials (BOM)
List of all components/modules used in the project.
This was automatically generated using Kicad's BOM generator.

Reference	|Value	|Footprint	|Qty	|
|--------|--------|--------|--------|
C1	|C	|	|1	|
C2	|C_Polarized	|	|1	|
D2,D3,D4,D5,D6,D7,D8,D9,D10,D11,D12,D13,D14,D15	|LED	|LED_THT:LED_D1.8mm_W3.3mm_H2.4mm	|14	|
J1	|Conn_01x07_Socket	|Connector_Molex:Molex_KK-396_5273-07A_1x07_P3.96mm_Vertical	|1	|
J2	|Conn_01x09_Socket	|Connector_Molex:Molex_KK-254_AE-6410-09A_1x09_P2.54mm_Vertical	|1	|
R1,R2	|R	|	|2	|
SW1,SW2,SW3,SW4,SW5,SW6,SW7,SW8	|SW_Push_Dual	|SW_PUSH_6mm_H5mm	|8	|
U1	|TSSP58038	|OptoDevice:Vishay_MINICAST-3Pin	|1	|


## SOFTWARE
The code  for this project  can be found in "/software/UV_timer/UV_timer.ino"

The timing is handled by arduino's millis().

If precise timing is required of very short durations the Atmega's internal timers can be used .


## End Note

NOTE:The labels of the buttons and their use are modified in v1 of this project.i.e

    - PAUSE BUTTON (SWx) IS UNUSED 
    instead ON BUTTON (SWy) is used for start/pause.


>.

The hardware, logic, and code are by no means the most efficient and masterfully designed. Thus any modifications and improvements are highly encouraged.


