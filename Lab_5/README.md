# Lab # 5 - Full Adder
# Table of contents
1. [Introduction](#introduction)
2. [Schematics](#paragraph1)
   
   1.[NAND](#NAND)
   
   2.[NOT](#NOT)
   
   3.[XOR] (#XOR)

   4.[Full Adder] (#Full Adder) 
4. [Layout](#paragraph3)


   1.[NAND](#NAND)
   
   2.[NOT](#NOT)
   
   3.[XOR](#XOR)
   
   4.[Full Adder](#Full Adder)
4. [Simulations](#paragraph3)
   
   1.[NAND](#NAND)
   
   2.[NOT](#NOT)
   
   3.[XOR](#XOR)
   
   4.[Full Adder](#Full Adder)
## Introduction <a name="introduction"></a>
    1. The objective of Lab 5 was to create a NAND, NOT, and XOR schematic and layout and use that to create a Full Adder schematic and layout using all three gates and routing them together as well as simulating the timings and truth tables of the different gates.
## Schematics <a name="Schematics"></a>
   1. This section covers the schematics of the NAND, NOT, XOR, and Full Adder in the sub sections provided below.
## NAND <a name="NAND"></a>
   1. Figure 1 below shows the schematic of a two input NAND gate with two PMOS transistors with both a width of 6 and a length of 2 and two NMOS transistors with a width of 6 and length of two using A and B as inputs and Y as the output and the reason why the NMOS looks different is because the NMOS were shifted left to Right instead of the regular configuration.
      
<img width="834" alt="NAND" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/33e8a564-6e95-4f17-b120-ca0a16549b8f">



      Figure 1: Schematic of NAND Gate
## NOT <a name="NOT"></a>
   1. Figure 2 below shows the schematic of a Not gate or a Inverter by using a PMOS with a width of 6 and a length of 2 and a NMOS with a width of 6 and a length of 2 in a different configuration regarding the position and having A as a input and Y as a output.

   <img width="750" alt="NOT" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/9506a191-af6c-442f-9d07-af186cc2272c">

 
 

       Figure 2: Schematic of NOT/Inverter Gate
## XOR <a name="XOR"></a>
   1. Figure 3 below shows the work done on paper of simplifying the number of transistors down to the simplest number of transistors possible and it shows some work done to get to the layout using Euler path and Stick diagrams. Figure 4 shows the schematic of the XOR created with 4 PMOS with the width of 6 and length of 2 and 4 NMOS with a width of 6 and length of 2 in a different configuration of position all wired together and another inverters that use the inputs A and B each with one PMOS and one NMOS with width of 6 and length of 2.

![HandCalculations for XOR](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/5a79a2d3-bf10-4917-8778-e3e652d0fe4f)


      Figure 3: HandCalculations of XOR including EULER PATH, STICK DIAGRAMS, and Simplifications
<img width="788" alt="XOR" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/1c943a23-1670-4302-9780-7494d96c8dfa">

   Figure 4: Schematic of XOR GATE
## Full Adder <a name="Full Adder"></a>
   1. Figure 5 below shows the schematic of Full Adder using the 3 NAND gates as icons and 2 XOR gates as icons and use three inputs A, B, and Cin and the outputs S and Cout and wire the schematic according to the tutorial that was given to us.

<img width="839" alt="Full adder" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/86385325-981e-46c7-8506-1b9b629a06b2">


      Figure 5: Schematic of Full Adder using 3 XOR and 2 NAND Gates
      
## Layout <a name="Layout"></a>
   1. This section contains the layouts of the Nmos, Final_IC_Not_ESD, pActive_nWell, pWell_nActive, Pad_ESD, Padframe_ESD, and Final_IC_ESD in the sub sections provided below.
## NAND <a name="NAND"></a>
   1. Figure 6 below shows the layout of NAND which is two PMOS with a P-active between the two PMOS and a P-active on the end of each of the PMOS transistors combined with two NMOS with N-actives between the two NMOS transistors and one N-active on each end of the NMOS transistors and the PMOS should be connected with VDD which is a n-well and the NMOS should be connected with gnd which is p-well and the inputs B and A should be connected to the NMOS and PMOS transistor on the gate. This should look very similar to the NAND gate layout in the tutorial.
      
<img width="609" alt="NAND" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/dbc29ab2-79c9-4da2-959f-9afe3afcdeb0">


      Figure 5: Layout of NAND
## NOT <a name="NOT"></a>
   1. Figure 7 below shows the layout of the NOT which is a PMOS transistor with two p-active one on each end and a NMOS transistor with two n-active one on each end and the PMOS is connected to the n-well which is vdd and the NMOS connected to the p-well which is gnd and the input A is connected to the PMOS and NMOS and the output Y connecting the PMOS and NMOS and this should be very similar to the tutorial in the layout.

<img width="527" alt="NOT" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/02929ed5-4e9a-450c-88bc-5ee50be7c3e9">


      Figure 7: Layout of NOT GATE
## XOR <a name="XOR"></a>
   1. Figure 3 above shows the handcalculations and work to get to the layout of the XOR using Euler path and Stick diagrams and Figure 8 below shows 4 PMOS transistors in the middle with p-actives between two PMOS transistors and P-actives on the ends of the PMOS transistors and 4 NMOS transistors also with n-actives between two NMOS transistors and n-actives on the ends of the NMOS transistors. To the left of the middle part of the layout is a Not gate layout for input A and to the right of the middle part of the layout is a Not gate layout for input B. The NMOS transistors are connected to the ground which is the p-well and the PMOS transistors are connected to vdd which is the n-well. The layout of the XOR should be very similar to the layout in the tutorial.
      
<img width="809" alt="XOR" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/bf87a26b-0f5f-4259-a365-f8a1e96c7d17">



      Figure 8: Layout of XOR GATE
## Simulations <a name="Simulations"></a>
   1. This section contains the layouts of the Nmos, Final_IC_Not_ESD, pActive_nWell, pWell_nActive, Pad_ESD, Padframe_ESD, and Final_IC_ESD in the sub sections provided below.
## Inverter_1 and Inverter_2 without load <a name="Inverter_1 and Inverter_2 without load"></a>
   1. Figure 7 below shows the simulation graph of the inputs and the both outputs of Inverter_1 and Inverter_2 and based on the figure below I could observe that while the voltage input is linear but the two outputs of Inverter_1 and Inverter_2 are not linear and are kind of sideways x^3 graph.
<img width="1268" alt="Schematic of two inverters without the load" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/544b90d8-67e6-460f-b482-692fb5428bf7">

      Figure 7: Simulation of Inverter_1 and Inverter_2 with a linear input
## Inverter_1 and Inverter_2 with load <a name="Inverter_1 and Inverter_2 with load"></a>
   1. Figure 8 and Figure 9 below shows the simulations of Inverter_1 and Inverter_2 with a Capacitor load of 1pF, 10pF, and 100pF and as you can see from the Figures below the outputs are going all over the place and is not stable at all. In Figure 10 below you can see the simulations of Inverter_1 and Inverter_2 with a Capacitor load of 100fF and the outputs of the Inverter_1 and Inverter_2 is less unstable and you see that it curves and starts to stablize.
<img width="1269" alt="Schematic of two inverters with capacitator load for Vout1 with Vin" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/233c5fcd-5f41-4e92-8f44-554139755280">

      Figure 8: Simulations of Inverter_1 output and input at 1pF, 10pF, and 100pF
<img width="1264" alt="Schematic of two inverters wih capacitator load for Vout2 with Vin" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/666152c1-0729-4f4c-8741-16881ef880cc">

      Figure 9: Simulations of Inverter_1 output and input at 1pF, 10pF, and 100pF
<img width="1266" alt="Schematic of two inverters with capacitator load at 1f 10f and 100f" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/f9e4c940-7633-400a-ac16-6ba48a74ed00">

      Figure 10: Simulations of both Inverter_1 and Inverter_2 outputs and input at 100fF
## Challenges <a name="Challenges"></a>
   1. The challenges of this lab was doing the routing for the second inverter because you had to be very careful with the spacing and how you orient your components or else you would get alot of errors and looking at the tutorial and trying to do Inverter_2 layout was very difficult but the rest of the lab was pretty straight forward.
## Future Plans <a name="Future Plans"></a>
   1. In the future there will be a lab on making a Full Adder I believe.




      




      









 



 



 
