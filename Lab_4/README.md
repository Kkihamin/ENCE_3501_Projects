# Lab # 4 - Inverters
# Table of contents
1. [Introduction](#introduction)
2. [Schematics](#paragraph1)
   
   1.[Inverter_1](#Inverter_1)
   
   2.[Inverter_2](#Inverter_2)
   
   3.[Combination of Inverter_1 and Inverter_2 without load] (#Combination of Inverter_1 and Inverter_2 without load)

   4.[Combination of Inverter_1 and Inverter_2 with load] (#Combination of Inverter_1 and Inverter_2 with load) 
4. [Layout](#paragraph3)


   1.[Inverter_1](#Inverter_1)
   
   2.[Inverter_2](#Inverter_2)
## Introduction <a name="introduction"></a>
    1. The objective of Lab 4 was to create two inverters inverter_1 which is just a basic inverter in CMOS and a inverter_2 which is a bigger inverter CMOS using inverter_1 and simulationing it on LT Spice together without the load and with the load to explore the behavior of the circuit.
## Schematics <a name="Schematics"></a>
   1. This section covers the schematics of the Inverter_1, Inverter_2, combination of Inverter_1 and Inverter_2 without a load, combination of Inverter_1 and Inverter_2 with loads in the sub sections provided below.
## Inverter_1 <a name="Inverter_1"></a>
   1. Figure 1 below shows the schematic of the basic inverter CMOS with a PMOS with a length of 6 and a width of 12 and a NMOS with a length of 6 and a width of 6. This is created by just inserting a PMOS and a NMOS component and then wiring it together with exports, a ground, inputs and outputs, and modifying the widths and lengths according to the lab tutorial.
      
<img width="831" alt="Inverter_1" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/c007d1b6-05d9-4a7e-9892-5f21bac3a7f0">


      Figure 1: Schematic of CMOS of Inverter_1
## Inverter_2 <a name="Inverter_2"></a>
   1. Figure 2 below shows the schematic of a bigger inverter CMOS with a PMOS with a length of 6 and a width of 48 and a NMOS with a width of 6 and length of 24. This is created by just inserting a PMOS and a NMOS component and then wiring it together with exports, a ground, inputs and outputs, and modifying the widths and lengths according to the lab tutorial.
 
 <img width="732" alt="Inverter_2" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/96d2aea0-6509-4965-8c30-4f03ef3e7286">

       Figure 2: Schematic of CMOS Inverter_2
## Combination of Inverter_1 and Inverter_2 without load <a name="Combination of Inverter_1 and Inverter_2 without load"></a>
   1. Figure 3 below shows the schematic of the Inverter_1 and Inverter_2 connected together as a circuit without a capacitator load. This is created by inserting the icons of Inverter_1 and Inverter_2 and using exports, ground, and labels according to the lab tutorial provided for this lab. Also, don't forget to set up the spice code with the C5 model and the code given in the tutorial.

      <img width="774" alt="Schematic of both inverters without capacitor load" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/0594b8c9-3fed-4b2f-b54f-7fc2ae62d4eb">

      Figure 3: Schematic of Inverter_1 and Inverter_2 without the load with spice code simulations
## Combination of Inverter_1 and Inverter_2 with load <a name="Combination of Inverter_1 and Inverter_2 with load"></a>
   1. Figure 4 below shows the schematic of the Inverter_1 and Inverter_2 connected together as a circuit with a capacitator load that is variable and changing depending which capacitator value is inputed. This is created by inserting the icons of Inverter_1 and Inverter_2 and using exports, ground, labels, and two capacitors for the label and set the value as {x} according to the lab tutorial provided for this lab. Additionally don't forget to set up the spice code with the C5 model and the spice code given in the tutorial since this is one of the things that will be simulated.

      <img width="835" alt="Schematic of both inverters with loads" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/60a90eb6-813a-47e6-a5a5-8725aaaf5031">

      Figure 4: Schematic of Inverter_1 and Inverter_2 with capacitor loads and Spice code simulations
      





## Layout <a name="Layout"></a>
   1. This section contains the layouts of the Nmos, Final_IC_Not_ESD, pActive_nWell, pWell_nActive, Pad_ESD, Padframe_ESD, and Final_IC_ESD in the sub sections provided below.
## Nmos <a name="Nmos"></a>
   1. Figure 8 below shows the layout of the Nmos with the gate, drain, source and the body completely routed.
      <img width="595" alt="Nmos_IV" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/f20e30a5-3e69-4175-8034-7e0caa000cb1">

      Figure 8: Layout of NMOS
## Final_IC_Not_ESD <a name="Final_IC_Not_ESD"></a>
   1. Figure 9 below shows the layout of the Final IC without the ESD and shows the NMOS layout in the middle of the padframe layout and the gate, drain, source, and body are wired to the different pins on the pads of the padframe.
      <img width="646" alt="final_ic_notESD" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/402b6601-9a7c-4e9b-a4c1-1b179bc82440">

      Figure 9: Layout of the Final_IC_Not_ESD
## pActive_nWell <a name="pActive_nWell"></a>
   1. Figure 10 below shows the layout of the pActive_nWell and the nWell is wired to a metal 1 pin on the top and the pActive on the bottom wired to a metal 1 pin as well.
      <img width="443" alt="pActive_nWell" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/e29cdc0b-00fa-45aa-aaf0-8e7d7c8b9bfa">

      Figure 10: Layout of the pActive_nWell
## pWell_nActive <a name="pWell_nActive"></a>
   1. Figure 11 below shows the layout of the pWell_nActive and the nActive is wired to a metal 1 pin on the top and the pWell on the bottom wired to a metal 1 pin as well.
      <img width="435" alt="pWell_nActive" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/ab9c2790-6ee1-49e6-b7e2-c085321ca494">

      Figure 11: Layout of the pWell_nActive
## Pad_ESD <a name="Pad_ESD"></a>
   1. Figure 12 below shows the layout of the Pad with ESD protection incorporated with a Pad layout and a common VDD and gnd created with two metal 1 connectors connected with a wire. Then a metal 1 to metal 2 contacts and a metal 1 pins to connect the pActive_nWell and pWell_nActive layouts with the pad layout and the vdd and gnd based on the instructions of the lab.
      <img width="455" alt="pad_esd" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/e92e82b8-558e-42eb-a492-6f334236fbe8">

      Figure 12: Layout of Pad_ESD
## Padframe_ESD <a name="Padframe_ESD"></a>
   1. Figure 13 below shows the layout of the Padframe with ESD protection created with a array of Pad_ESD layouts copy and pasted and then the gnd and VDD all wired together with metal 1 pins
      <img width="652" alt="padframe_esd" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/92172db6-b616-409c-a5d5-7eaa81413431">

      Figure 13: Layout of the Padframe_ESD
## Final_IC_ESD <a name="Final_IC_ESD"></a>
   1. Figure 14 below shows the layout of the Final Ic with ESD protection created from the Padframe_ESD layout and the Nmos layout routed together.
      <img width="665" alt="final_ic_esd" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/28cfa61f-886c-4982-b88d-de5db5d603d9">

      Figure 14: Layout of Final_IC_ESD
## Challenges <a name="Challenges"></a>
   1. The challenges of this lab was doing the Pad_ESD because the instructions I followed for the Pad_ESD was not the clearest to determine what needed to be routed and after some help I was able to successfully able to create the Pad_ESD and after the Pad_ESD was created the rest of the process was pretty straight forward and the hardest part was done.
## Future Plans <a name="Future Plans"></a>
   1. In the future if these IC's were actually being manufactured and fabricated the design and layout especially with the spacing would be very important but because this is not being manufactured and fabricated the spacing errors can be ignored.





      




      









 



 
