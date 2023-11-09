# Lab # 6 - DC-to-DC Converter
# Table of contents
1. [Introduction](#introduction)
2. [HandCalculation](#HandCalculation).
3. [Schematics](#paragraph1)
   
   1.[3-Charge Pump](#3-Charge Pump)
   
   2.[Ring_Oscillator](#Ring_Oscillator)
   
   3.[Regulator] (#Regulator)

   4.[DC-DC Converter] (#DC-DC Converter) 
4. [Layout](#paragraph3)


   1.[3-Charge Pump](#3-Charge Pump)
   
   2.[Ring_Oscillator](#Ring_Oscillator)
   
   3.[Regulator](#Regulator)
   
   4.[DC-DC Converter](#DC-DC Converter)
5. [Simulations](#paragraph3)
   
   1.[3-Charge Pump](#3-Charge Pump)
   
   2.[Ring_Oscillator](#Ring_Oscillator)
   
   3.[Regulator](#Regulator)
   
   4.[DC-DC Converter](#DC-DC Converter)
## Introduction <a name="introduction"></a>
    1. The objective of Lab 6 was to create a DC-to-DC Converter by combining three different circuits which are the 3-Charge Pump, Ring Oscillator, and Regulator. Before we build the DC-DC Converter we needed to understand what each of the separate circuits do individually. The 3-charge Pump has three inputs and basically is a circuit that starts at a low voltage and has the ability where the voltage rises as time goes on. The Ring Oscillator basically has a odd number of inverter gates and has the ability to switch between two different voltage levels and is commonly used in compact layout designs where there is the possiblity of noise. The Regulator circuit used in applications where there is need for more power and is a important circuit in power electronics and has the ability to keep a constant voltage level without any fluctuations in the input voltage. The only circuit I was familiar was the 3-Charge pump because over the summer during my internship I did have to write some test cases using Labview that interacts with NI TestStand regarding charge pump for a specific product and be able to step the voltage to like a maximum of like 200V but when I was writing the test case for the charge pump I did not have the best understanding of what the charge pump was actually doing on the hardware side because I was mostly visualizing using software programs and I think this particular lab gave me alot better understanding of the Charge pump, Ring oscillator, and Regulator. This was the most difficult lab assignment that was done in this class and there was alot of difficulties and frustrations when trying to complete this lab.
## HandCalculation <a name="HandCalculation"></a>
   1. While doing the 3-charge Pump and Regulator there were calculations involved before actually creating the schematic and the layout. First, the PMOS and NMOS transistors used in the 3-charge Pump, Ring Oscillator, and Regulator the width and length were doubled from the originally schematic that was shown in the Lab 6_intro pdf document because the original ratio 10/1 would prove to be a problem in the layout because it would complain that it violates the minimum dimensions for the technology I was using. Since the width and length were doubled the size of the n-well resistors used in 3-charge pump and regulator circuit would need to be calculated using the formula $\(Ldiv W) * Rsquare\$ which would equal 2M for the 3-charge pump circuit and 20M and 3M for the Regulator circuit and all the work to get to the width and length of the resistors is shown in Figure 1 below.




      




      









 



 



 
