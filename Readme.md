# UV TIMER

Your friendly neighbourhood timer.

----

### About the project
----

This project is a general purpose hardware timer based on Arduino.

It uses the `Arduino Nano` as the controller, `WE___  16*2 display` and push buttons to interface with the timer. 

The UV is driven by `IRFZ44N mosfet`and two `L7805CV regulators` are placed in parallel to help provide current for heavy loads.

The UV Timer can be powered by a 12V or 5V adapter. 

A jumper (Jx) is provided that can be used to set the voltage for the load (5V or 12V).

![UV TIMER DEMO ](https://github.com/sam-prc-404/UV_timer/Gallery/ "UV TIMER DEMO ")


## HARDWARE

### Schematic and PCB design
The schematic and PCB for this project was designed using [Kicad EDA](https://www.kicad.org/).

->Schematic "/././.sch"

![UV TIMER SCHEMATIC ](https://github.com/sam-prc-404/UV_timer/Gallery/ "UV TIMER SCHEMATIC DIAGRAM")
>*INSERT SCHEMATIC PIC HERE*

-> PCB "/././.pcb"

![UV TIMER PCB ](https://github.com/sam-prc-404/UV_timer/Gallery/ "UV TIMER PCB DESIGN")
>*INSERT PCB PIC HERE*

### PCB Fabrication
Fabrication of the PCB for this project was done in-house at [@Robotics Club,Pulchowk Campus](https://robotics.pcampus.edu.np/). 
    
The fabrication method and guide used can be found [*here*](https://github.com/sam-prc-404/ "PCB Fabrication method")

![UV TIMER PCB FAB BACK PIC](https://github.com/sam-prc-404/UV_timer "Fabricated PCB Back")
> PCB BACK PIC

![UV TIMER PCB FAB FRONT PIC ](https://github.com/sam-prc-404/UV_timer "Fabricated PCB Front")
> PDB FRONT PIC


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
The code  for this project  can be found in [UV_Timer/Software/UV_timer.ino ](https://github.com/sam-prc-404/UV_timer "UV TIMER CODE")

The timing is handled by arduino's `millis()`.

If precise timing of very short durations is required the Atmega's internal timers can be used.



## End Note


<div style="background-color: #CE2029; padding: 10px; border-radius: 6px;">
  <strong>⚠️ NOTE ⚠️: </strong>  The labels of the buttons and their functions do not line up in v1 of this project. Please be aware of this issue while using the application.
</div>
<br>

> `PAUSE BUTTON` (SWx) IS UNUSED , instead `ON BUTTON` (SWy) is used for start/pause.

***

>The hardware, logic, and code are by no means the most efficient and professionally designed. There still exits many faults and improvements . Thus any modifications and improvements are highly encouraged.

***
