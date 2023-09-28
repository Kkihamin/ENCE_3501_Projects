# David Ki
# ENCE 3501
# 09/27/2023

# Lab # 1 - DAC 


## HandCalculations

  1. This is the image of the 5 bit DAC used to calculate the output resistance below.
     ![output resistance for DAC](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/86b7a7d6-bf25-4649-9bf1-e70af1053feb)
     
Figure 1: The output resistance calculation of the 5 bit DAC

The output resistance came out to be 10kohms.

2. This is the image of the hand calculations of the delay if a 5 bit DAC has a 10pF capacitator load below.
   
![handcalculations for load and delay](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/7edaf89c-9448-4648-b8bb-cf34e3ca3beb)

Figure 2: The delay of the 5 bit DAC with 10pF capacitator load 

Based on Figure 2 above I did 0.7*(10 X 10^3)*(10 X 10^-12) = 70ns

3. Figure 3 below shows the delay I got on the simulation through LtSpice

   <img width="1275" alt="LT Spice for capacitator 2v DAC" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/07307801-9370-46ee-b051-5cb828728bc6">

   Figure 3: Delay of 70ns shown in the simulation

4. The image below shows the simulation of the 5 bit DAC with a 10k load resistor at 2 volts.

   <img width="1273" alt="voltage simulation with resistor load for 2v" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/b23fd1ee-3d8a-44ec-b2ba-4aada5a9ee1a">

   Figure 4: Simulation on 5 bit DAC with 10k load at 2 volts

 ![handcalculations for load and delay](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/7fd158c7-b60c-43ed-ace9-2b7e585935e1)

   Figure 5: Handcalculation on 5 bit DAC with load 10k
<img width="1277" alt="simulation of DAC with load at 1V" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/0d66f42a-bd12-4dab-a9c0-ab9bfe0fed7d">
   
  Figure 6: Simulation of the DAC with 10k load at 1V

  <img width="1267" alt="schematic with resistor load at 3V" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/d029665c-7de2-4752-9b4f-ef438e457bdf">

  Figure 7: Simulation of the DAC with 10k load at 3V

  <img width="1277" alt="DAC with load for 4V" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/fc6be308-92b3-4ff0-b906-eea84592e5fb">

  Figure 8: Simulation of the DAC with 10k load at 4V.


   I noticed as the voltage I input increased the voltage output increased and the current decreased. For example, at 1v the current was 50uA but at 2V the current went down to 100uA of current.

## Schematics

The following figures are the schematics from the foundation R_Divider to the 5 bit DAc to the 5 bit DAC with the resistor load or capacitator load

<img width="847" alt="R_Divider schematic" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/d654da31-8e92-4f9d-b741-09b07a56c27b">
<img width="470" alt="R_divider simulation results" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/ecf3d14e-d8a5-40b6-9d0f-1e0fb8d99b2e">


Figure 9: Schematic of R_Divider for the foundation of the 5 bit DAC and the simulation values

<img width="637" alt="5 bit DAC without load" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/95cdd3c1-e875-4387-a188-780ea7aaab6e">
<img width="589" alt="DAC input voltage with 5 volts" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/b3a94c91-b53d-43de-9f29-127977ba16a5">

Figure 10: Schematic of 5 bit DAC created from the icon of R_Divider and simulation values

<img width="975" alt="circuit for DAC" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/821ffb1f-142e-4330-91ae-102538e342ff">

Figure 11: Schematic of 5 bit DAC as a icon and most of the inputs grounded

<img width="587" alt="DAC with resistor load schematic" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/979b7de8-fc04-4cd1-bf67-9b588f13f3ae">

Figure 12: Schematic of 5 bit DAC with a 10k load resistor

All the other schematics I might of not put on here along with the simulations have all been verified.
## Layout
The following figures below are the layout of the R-divider and the DAC.

<img width="654" alt="layout of R_Divider" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/725908bd-7fe1-4388-9f7f-240a2075d3dc">

Figure 13: Layout of the R_Divider

<img width="630" alt="layout of DAC without load" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/701a0b48-77d1-4ca7-a1bd-9db5b8d87cc6">

Figure 14: Layout of the DAC

The Width and length were determined by R = ρ/t * L/W = Rsquare * L/W 








   










 
