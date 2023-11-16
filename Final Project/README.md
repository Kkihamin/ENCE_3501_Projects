# Lab - Final Project - Counter16
# Table of contents
1. [Introduction](#introduction)
2. [Schematics](#paragraph1)
   
   1.[And gate](#And gate)
   
   2.[Inverter](#Inverter)
   
   3.[D Flip Flop] (#D Flip Flop)

   4.[Counter16] (#Counter16) 
4. [Layout](#paragraph3)


   1.[And gate](#And gate)
   
   2.[Inverter](#Inverter)
   
   3.[D Flip Flop](#D Flip Flop)
   
   4.[Counter16](#Counter16)
5. [Simulations](#paragraph3)
   
   1.[And gate](#And gate)
   
   2.[Inverter](#Inverter)
   
   3.[D Flip Flop](#D Flip Flop)
   
   4.[Counter16](#Counter16)
## Introduction <a name="introduction"></a>
    1. The Final project was the idea of the creating a simple VSM microprocessor and every student in the class picked a different component that would hopefully be integrated together to create VSM microprocessor that is a very simple microprocessor. For my final project I attempted to create a successfully working Counter16 component that uses a And gate, 4 D Flip Flops, and Inverter gates. Given a ElectricVLSI template with all of the components needed to create the Counter16 I thought creating the Counter16 would be easier to implement than it actually turned out to be while trying to implement the Counter16. This implementation gave me an idea and realized how difficult it is to actually create even single components and it takes a lot of time effort and patience to implement VLSI projects.
## Schematics <a name="Schematics"></a>
   1. This section shows the Schematics of the And gate, Inverter gate, D Flip Flop, and Counter16. I used the mudlib ElectricVLSI template that had the And gate, Inverter gate, and D Flip Flop. The specific group of components I used are and2_1x, flopr_c_1x, and inv_1x. The Counter16 utilizes all these different components from the template and integrates them together to make the Counter16 described in much detail below. 
## And gate <a name="And gate"></a>
   1. The first I did was open up the mudlib library template with all the components necessary for the final project on ElectricVLSI. Next, I scrolled down till I got to all the different And gates and I specifically picked and2_1x because for the Counter16 I had a two input And gate with one output which this specific template satisfies the requirements for the Counter16. Then I right clicked on the cell and then hit copy and then I copied the entire cell group to my counter16 project. Finally, I set spice models for all the PMOS and NMOS transistors to P_1u or N_1u based on the cmosedu_models.txt file since I was using vdd as 5 volts. Figure 1 below shows the schematic of the And gate that I used.
      
      <img width="723" alt="And_gate" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/278a891d-4a3b-4ab1-be17-8126e1a433a7">



       Figure 1: Schematic of And Gate
## Inverter <a name="Inverter"></a>
   1. The first I did was open up the mudlib library template with all the components necessary for the final project on ElectricVLSI. Next, I scrolled down till I got to all the different Inverter gates and I specifically picked inv_1x because for the Counter16 I had a one input inverter gate with one output which this specific template satisfies the requirements for the Counter16. Then I right clicked on the cell and then hit copy and then I copied the entire cell group to my counter16 project. Finally, I set spice models for all the PMOS and NMOS transistors to P_1u or N_1u based on the cmosedu_models.txt file since I was using vdd as 5 volts. Figure 2 below shows the schematic of the inverter gate that I used.
      
      <img width="728" alt="Inverter_gate" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/ceed5eff-256f-49ff-b4b3-8126a5f877ae">



      Figure 2: Schematic of Inverter Gate
## D Flip Flop <a name="D Flip Flop"></a>
   1. The first I did was open up the mudlib library template with all the components necessary for the final project on ElectricVLSI. Next, I scrolled down till I got to all the different D flip flops and I specifically picked flopr_c_1x because for the Counter16 I had two clocks, one reset on the bottom, input d and output q and this template was the only one that satisfied the requirements for the Counter16. Then I right clicked on the cell and then hit copy and then I copied the entire cell group to my counter16 project. Then, when I ran F5 to check if there were errors I did in fact get errors which was the ph1 and ph2 had characteristics of a clock but on the icon the ph1 and ph2 had characteristics that were unknown and ElectricVLSI was getting confused because the characteristics of ph1 and ph2 being clocks on the schematic did not match on the icon. Finally, I set spice models for all the PMOS and NMOS transistors to P_1u or N_1u based on the cmosedu_models.txt file since I was using vdd as 5 volts. Figure 3 below shows the schematic of the D Flip Flop that I used.
      
<img width="665" alt="D flip flop" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/90630b70-95b1-44e1-aa6c-5f07668bbb7e">


Figure 3: Schematic of D Flip Flop
## DC-DC Converter <a name="DC-DC Converter"></a>
   1. The schematic of the DC-DC converter is shown below in Figure 5 but I did not take the time to simulate the DC-DC converter because it did not actually work on my end and I did not want to spend too much time trying to figure why the DC-DC Converter simulations were not working and I wanted to focus more on the final project. If I did not have a final project I would of tried to figure out how to simulate the DC-DC Converter.
      
<img width="839" alt="DC-DC" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/ba875236-604f-4bbf-8316-d9b915f39702">

Figure 5: Schematic of DC-DC Converter without Spice Code
## Layout <a name="Layout"></a>
   1. This section shows the Layouts of the 3-Charge Pump, Ring Oscillator, Regulator, and DC-to-DC Converter. The Layouts of the 3-Charge Pump, Ring Oscillator, Regulator, and DC-to-DC Converter does not have any simulations because I was getting errors when trying to simulate this and it just was not working for me for some reason. I did keep the capacitors and resistors in the layouts even though the capacitors and resistors should not be included in the layout because the size of these components are too large to put on the layout. Also, another error I faced was the NCC still did not match up for the layouts because the exports on the output of each of the circuits were not showing up even though I did add them and I could not figure it out and tried to redo it multiple times but the error did not disappear. All the layouts of the circuits are shown below.
## 3-Charge Pump <a name="3-Charge Pump"></a>
   1. The layout of the 3-Charge Pump was created using 4 NMOS transistors all with a width of 20 and a length of 2, 4 100uF capacitors, and 1 2M ohm resistor with the width of 119.76 and length of 20. I did the layout in the same structure as the schematic and I looked at the schematic to see and understand how to wire things together in the layout. The only problems are that it is not feasible to put the capacitors on the layout because the size for 100uF capacitors would be way too large and the simulations do not run because the NCC for the export on the output of this circuit does not exist in the layout and there are other problems with the simulations that I was not able to figure out. Also, if the voltage wanted to be higher than what it actually is shown when I run the simulation there should be two more transistors and one more capacitor to make a 5 stage pump circuit. Also, the current layout of the 3-Charge pump is different because I replaced the capacitors with wires and named them to see if it would fix the NCC and simulate but it did not work. Figure 6 below shows the layout of 3-Charge Pump looking exactly like the schematic.

   <img width="534" alt="3-stage charge pump" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/7c1f619e-38a1-450b-b7c2-d0f7aca10597">

   Figure 6: Layout of 3-Stage Charge Pump not done Exactly Correct
## Ring_Oscillator <a name="Ring_Oscillator"></a>
   1. The layout of the Ring Oscillator was created using 4 Inverter layouts dragged in from a previous lab, 1 NAND layout dragged in from a previous lab, and 3 poly capacitors that are 10uF. I did the layout in the same structure as the schematic and I looked at the schematic to see and understand how to wire things together in the layout. The only problems are that it is not feasible to put the capacitors on the layout because the size for 10uF capacitors would be way too large and the simulations do not run because the NCC for the export on the output of this circuit does not exist in the layout and there are other problems with the simulations that I was not able to figure out. Figure 7 below shows the layout of Ring Oscillator looking exactly like the schematic.

      <img width="830" alt="Ring_Oscillator" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/d9682bfb-44b4-416f-85a5-71b12fb4dce5">

      Figure 7: Ring Oscillator Layout
## Regulator <a name="Regulator"></a>
   1. The layout of the Regulator was created using two inverter layouts dragged in from a previous lab, 2 PMOS transistors with P-active connectors, 1 NMOS transistor with n-active connectors, and one 20M resistor and one 3M resistor. I did the layout in the same structure as the schematic and I looked at my schematic to see and understand how to wire things together in the layout. The problem was that it is not very good to put the resistors in the layout because they are pretty big and the simulations ran once on the layout and then after that one time if stopped working and the NCC export for the output was a issue for this layout as well. Figure 8 below shows the layout of the Regulator looking similar to the schematic.

   <img width="765" alt="Regulator" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/4035d81e-2ceb-442c-8107-2b469c8ca5d2">

   Figure 8: Layout of Regulator
## DC-DC Converter <a name="DC-DC Converter"></a>
   1. The layout of the DC-DC Converter was created by importing the layouts of the  3 stage charge pump, ring oscillator, and regulator and wiring them together exactly like the schematic but this layout of the DC-DC Converter is not the most accurate because there were problems in the previous layouts so the simulations, NCC, and layout itself would not be exactly the best representation. Due to the limited time I had to dedicate time to this lab and dedicating more time to the final project made me not worry about the layout of the DC-DC Converter from not working with the simulation. Figure 9 below shows the layout of the DC-DC Converter.

      <img width="718" alt="DC-DC" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/40d31ba4-a91a-4fba-b196-34cb1c66fa84">
      
      Figure 9: Layout of DC-DC Converter
## Simulations <a name="Simulations"></a>
   1. This section shows the Simulations of the 3-Charge Pump, Ring Oscillator, and Regulator. The simulations are only from the schematic for the 3-charge pump, ring oscillator, and the        regulator but there is no simulation for the DC-to-DC Converter due to lack of time and focusing more on the final project. The layout simulations did not work so I was kind of 
      frustrated because there were so many errors and I was overwhelmed but I was not able to figure out why the simulations for the layouts were not working.
## 3-Charge Pump <a name="3-Charge Pump"></a>
   1. The Simulation of 3-Charge Pump for the schematic is shown in Figure 10 below. The problem wih this simulation is the 3-Charge Pump does not rise up to the correct voltage and in my case the 3- Charge Pump rose but stop at a number below 1V and one reason I could of done to raise the voltage is make it a higher stage charge pump and mess with the periods more but due to the lack of time and wanting to focus on the final project I just kept the simulation as it was originally. If you see other images of the simulations that say layout it is actually not the simulation of the layout and just a duplicate copy from the schematic simulation.

<img width="1279" alt="Transient for 3 charge pump for schematic" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/bf1e7b5f-4d92-4776-a711-3f533d3da906">


   Figure 10: Simulation of 3 Charge Pump failing to meet the correct Voltage
## Ring_Oscillator <a name="Ring_Oscillator"></a>
   1. The simulation of ring oscillator for the schematic is shown in Figure 11 below. There are actually not any problems with this simulation of the ring oscillator because it shows the pulse waveforms correctly but it does not show anything in the layout which is the problem. The one thing that could be improved for the ring oscillator is more accuracy in the pulse waveforms.

<img width="1270" alt="schematic simulation for ring oscillator" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/9cf32bac-d463-4b17-8f7c-a0651963ae0d">

     Figure 11: Simulation of Ring Oscillator
## Regulator <a name="Regulator"></a>
   1. The simulation of the Regulator is shown in Figure 12 below. The problem is I got a sine wave for the simulation of the schematic and I was uncertain whether that is what the waveform of the Regulator is suppose to look like and the layout only ran once successfully but I was unable to capture the simulation of the layout but I got the same waveform from what I remember.

<img width="1264" alt="Regulation simulation for schematic" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/d7465161-33ef-4f77-ab27-b26ff0a97a75">

Figure 12: Simulation of Regulator
## DC-DC Converter <a name="DC-DC Converter"></a>
   1. For the simulations regarding the schematic and layout of the DC-DC converter I did not have because I ran into problems in simulating the layout and some schemtics of the previous circuits that I determined that the simulation for DC-DC Converter would fail and not simulate but if I had some time and not a final project to worry about I would have definitely tried to simulate this DC-DC Converter and I would of tried to fix my issues that I ran into above.
## Challenges <a name="Challenges"></a>
   1. The challenges with this lab was there was limited information and alot of the information I had to figure out and try to find a working solution especially with the poly poly capacitor changing the sizes to double the width and the length after messing with the layout and messing with spice code and simulations. Also, another challenge was just knowing a lot more things about the ElectricVLSI software. Personally I think this lab was a really good learning experience and lab and I am not sure if I did everything completely right but I think this was definitely a good learning experience.
## Future Plans <a name="Future Plans"></a>
   1. My future plans will be working on a Final project for VLSI and making a 16 bit counter using a template that has alot of components created and using D flip flops to implement a counter and wrapping up the rest of the work for this class.


 






      









      




      









 



 



 
