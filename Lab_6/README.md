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
   1. While doing the 3-charge Pump and Regulator there were calculations involved before actually creating the schematic and the layout. First, the PMOS and NMOS transistors used in the 3-charge Pump, Ring Oscillator, and Regulator the width and length were doubled from the originally schematic that was shown in the Lab 6_intro pdf document because the original ratio 10/1 would prove to be a problem in the layout because it would complain that it violates the minimum dimensions for the technology I was using. Since the width and length were doubled the size of the n-well resistors used in 3-charge pump and regulator circuit would need to be calculated using the formula $\(Ldiv W) * Rsquare\$ which would equal 2M for the 3-charge pump circuit and 20M and 3M for the Regulator circuit and all the work to get to the width and length of the resistors is shown in Figure 1 below. There are Poly 1 to Poly 2 capacitator used in the circuits above but I tried to find the formulas and tried to determine the size of the capacitators but I was not able to successfully determine the size of the capacitator and there was not enough time to calculate the size of the capacitators.
![HandCalculations](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/f357bbb0-a8b7-4dc0-82fc-f17c45f3361e)

Figure 1: HandCalculations for 3-Charge Pump and Regulator Resistors
## Schematics <a name="Schematics"></a>
   1. This section shows the Schematics of the 3-Charge Pump, Ring Oscillator, Regulator, and DC-to-DC Converter. The Schematics of the 3-Charge Pump, Ring Oscillator, Regulator, and DC-to-DC Converter were a little bit different from the Schematics we did in the previous labs because they were alot larger and lot more complex to create because I had to think about the layout while doing the schematic so that when I was doing the layout it would not be very difficult to do the layout based on the schematics that I create. The lab 6 tutorial with the sample schematics of the 3-Charge Pump, Ring Oscillator, Regulator, and DC-to-DC Converter helped a little bit but at the same time made it difficult because it kind of gave me the preconception that if I followed the sample schematics given I would be fine and there would be no problems but this i quickly figured out while making the schematic.
## 3-Charge Pump <a name="3-Charge Pump"></a>
   1. The first I did before creating the schematic of 3-Charge pump was calculate the width and length. I used the equation $\(L div W) * Rsquare\$ and for this equation I realized that I needed to either assume the length or width to get the other dimension so I decided the length to be 20 and I knew the Rsquare was equal to 835 from previous assignments and looking back at my notes so I multiplied 835 by 20 which equals to 2M. Next, I divided 2M and 16,700 to get a width of 119.76. Then, I looked at the special cmos text file to decide what the spice model for the NMOS and PMOS should be based on whether the vdd is 1V or 5V which in this case we are using 1V which makes the spice model N_50n and P_50n. Then, I used 4 NMOS transistors with width of 20 and a length of 2 and 4 100u capacitors but I did not change the size on the 100u capacitors because I knew the poly capacitors on the layout would be to large to fit on the layout and I just left it in the schematic to visualize that there are capacitors being used in the 3-stage pump circuit. Finally, wire all the components together using the Lab 6 intro document like the sample circuit of the 3-stage pump given in the document. Figure 2 below shows the schematic of the 3-Stage pump circuit.
      
      <img width="832" alt="3-stage charge pump" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/811b1edb-48d5-4b1e-b879-7c34cc20559b">


       Figure 2: Schematic of 3-Charge Pump
## Ring_Oscillator <a name="Ring_Oscillator"></a>
   1. The first I did before creating the schematic of Ring_Oscillator was to import one NAND, and four Not gates from a previous lab where I had already created a NAND and Not gate. Next, I changed all the spice models for the transistors on the NAND and Not schematic to N_50n and P_50n based on the special purpose CMOS text file. Then, I got 3 10uF poly 1 to poly 2 capacitors and I did not change the size of the poly capacitors because I knew the size of the capacitors changed on the schematic would need to be reflected in the layout and would take a lot more time and I wanted to focus more on the final project. Finally, wire all the components together using the Lab 6 intro document like the sample circuit of the Ring_Oscillator given in the document. Figure 3 below shows the schematic of the Ring_Oscillator circuit.
      
      <img width="843" alt="Ring_Oscillator" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/bce7b774-e8e9-4e12-8bf1-8ba05866fb53">


      Figure 3: Schematic of Ring_Oscillator
## Regulator <a name="Regulator"></a>
   1. The first I did before creating the schematic of Regulator was calculate the width and length. I used the equation $\(L div W) * Rsquare\$ and for this equation I realized that I needed to either assume the length or width to get the other dimension so I decided the length to be 200 and I knew the Rsquare was equal to 835 from previous assignments and looking back at my notes so I multiplied 835 by 200 which equals to 20M. Next, I divided 20M and 167,000 to get a width of 119.76. I used the equation $\(L div W) * Rsquare\$ for the second resistor as well and for this equation I realized that I needed to either assume the length or width to get the other dimension so I decided the length to be 50 and I knew the Rsquare was equal to 835 from previous assignments and looking back at my notes so I multiplied 835 by 50 which equals to 3M. Next, I divided 3M and 41,750 to get a width of 71.895. Then, I looked at the special cmos text file to decide what the spice model for the NMOS and PMOS should be based on whether the vdd is 1V or 5V which in this case we are using 1V which makes the spice model N_50n and P_50n. Then, I used 2 PMOS transistors with width of 20 and a length of 40, 1 NMOS transistor with a width of 20 and a length of 2, 2 inverter gates used as a icon, and 2 N-well resistor one which is 20M and the other one being 3M. Finally, wire all the components together using the Lab 6 intro document like the sample circuit of the Regulator given in the document. Figure 4 below shows the schematic of the Regulator circuit.
      
<img width="838" alt="Regulator" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/126c1814-1889-4a57-a488-edac87302a41">

Figure 4: Schematic of Regulator Circuit
## DC-DC Converter <a name="DC-DC Converter"></a>
   1. The schematic of the DC-DC converter is shown below in Figure 5 but I did not take the time to simulate the DC-DC converter because it did not actually work on my end and I did not want to spend too much time trying to figure why the DC-DC Converter simulations were not working and I wanted to focus more on the final project. If I did not have a final project I would of tried to figure out how to simulate the DC-DC Converter.
      
<img width="839" alt="DC-DC" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/ba875236-604f-4bbf-8316-d9b915f39702">

Figure 5: Schematic of DC-DC Converter without Spice Code









      




      









 



 



 
