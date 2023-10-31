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
## Inverter_1 <a name="Inverter_1"></a>
   1. Figure 5 below shows the layout of Inverter_1 which is a PMOS combined with a NMOS as well as a N-actives, p-actives, N-Well, and a PWell. The one mistake I might of made that was one of the wires on the layout of Inverter_1 is not the same wire thickness and this is because I kept getting errors when I made it the same size and tried to move it around.
<img width="598" alt="Layout of Inverter_1" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/2a7176f4-fe22-4c0b-ba50-f7ddab7e4a45">

      Figure 5: Layout of Inverter_1
## Inverter_2 <a name="Inverter_2"></a>
   1. Figure 6 below shows the layout of the Inverter_2 which is a bigger layout than Inverter_1 and is created by inserting four of the Inverter_1 layouts over to this layout and then routing with N-acts, p-acts, p-well, n-well, and connectors to make the routing a easier process.
<img width="834" alt="Inverter_2 layout" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/cb4c4b4b-909c-4376-957d-74788a045101">

      Figure 6: Layout of Inverter_2
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




      




      









 



 



 
