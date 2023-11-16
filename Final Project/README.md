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
## Counter16 <a name="Counter16"></a>
   1. The schematic of the Counter16 was created from icons of one And gate, four D Flip Flops, and five inverter gates. Initially the And gate with inputs Ena and clk are connected to a inverter gate with a wire C1 which would be the ph1 which is just the clock and the output C2 which is the inverse of the clock ph1 which is what ph2 would be. Then, for every flip flop there would be a inverter where the output of the inverter would feed into the input d and connected to the ph1 of the next flip flop and the input of the inverter would be the output q and connected to ph2 of the next flip flop. Figure 4 below shows the schematic of the Counter16.
      
<img width="837" alt="counter_16" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/04f06673-ea30-4b6f-aab2-b3933b09a6b2">


Figure 4: Schematic of Counter16
## Layout <a name="Layout"></a>
   1.  This section contains the Layouts of the And gate, Inverter gate, D Flip Flop, and Counter16. The difficulties with the layout is figuring out how each of the individual components like the And gate, Inverter gate, and D Flip Flop work to be able to combine them together to make the Counter16. There were many iterations done to the layout especially the Counter16 because there were many errors like the wiring was not done correctly, missing exports, not very organized, and more. The layout of the Counter16 was the biggest and most complex layout I have done so far.
## And gate <a name="And gate"></a>
   1. Figure 5 below shows the layout of the And gate which is used in the Counter16. The And gate is used in the Counter16 to feed two inputs which are the clk and Ena which are related to the two clocks. This And gate below is used from the mudlib template for the component and2_1x and was already created for me to use.
      <img width="431" alt="And_gate" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/edd1d38f-4364-495d-9072-9aa0787d6f37">

      Figure 5: Layout of And Gate

## Inverter <a name="Inverter"></a>
   1. Figure 6 below shows the layout of the Inverter gate which is used in the Counter16. The inverter is used to connect to the four D Flip Flops and another way the Inverter gate is used is to invert the clock input compared to the other clock. This Inverter gate below is used from the mudlib template for the component inv_1x and was created to make the Counter16 easier to create to a certain point.
      
      <img width="502" alt="Inverter_gate" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/d833282c-ec5b-497d-9cae-3c2d97ad5cd2">

      Figure 6: Layout of Inverter Gate

## D Flip Flop <a name="D Flip Flop"></a>
   1.  Figure 7 below shows the layout of the D Flip Flop which is used in the Counter16. There are four D Flip Flop used in the Counter16. The four D Flip Flop used in the Counter16 make the Counter16 able to count up or down based on the pulses of the clocks. The four D Flip Flops are used from the mudlib template for the component flopr_c_1x and provided to make the Counter16 able to be created because if the D Flip Flop needed to be created from scratch it would of definitely been harder to implement the Counter16 in the given limited time.

   <img width="781" alt="D Flip Flop" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/46631c89-a792-49e9-acd5-942823e22f97">

      Figure 7: Layout of D Flip Flop

## Counter16 <a name="Counter16"></a>
   1. Figure 8 below shows the layout of the Counter16. The Counter16 was created by using four D Flip Flops, five Inverter gates, one And gate from the mudlib template provided with the layouts and schematics so I could just drag in the layouts of the different components needed to create the Counter16 and then wire all the components based on the schematic I created for the Counter16. This layout was the most difficult because if I needed to make changes to the schematic which I did then the layout would need to be redone from the very beginning. I made various edits to the schematic and layout about three or four times so the layout of Counter16 was done through various iterations.

      <img width="814" alt="Counter_16" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/19f22888-92d7-43d5-93ad-0d5726228412">

      Figure 8: Layout of Counter16
## Simulations <a name="Simulations"></a>
   1. This section shows the Simulations of the 3-Charge Pump, Ring Oscillator, and Regulator. The simulations are only from the schematic for the 3-charge pump, ring oscillator, and the        regulator but there is no simulation for the DC-to-DC Converter due to lack of time and focusing more on the final project. The layout simulations did not work so I was kind of 
      frustrated because there were so many errors and I was overwhelmed but I was not able to figure out why the simulations for the layouts were not working.
## And gate <a name="And gate"></a>
   1.
## Inverter <a name="Inverter"></a>
   1. 
## D Flip Flop <a name="D Flip Flop"></a>
   1. 
## Counter16 <a name="Counter16"></a>
   1. 
## Challenges <a name="Challenges"></a>
   1. 
## Future Plans <a name="Future Plans"></a>
   1.


 






      









      




      









 



 



 
