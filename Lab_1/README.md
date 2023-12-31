# Lab # 1 - DAC 
# Table of contents
1. [Introduction](#introduction)
2. [HandCalculations](#paragraph1)
    1. [Output Resistance](#Output Resistance)
    2. [delay with the 10pF capacitator load](#delay with the 10pF capacitance load)
    3. [Load of 10k resistor DAC](#Load of 10k resistance DAC)
3. [Schematics](#paragraph2)
    1. [R_Divider](#R_Divider)
    2. [5-bit DAC](#5-bit DAC)
    3. [5-bit DAC with 10pF load](#5-bit DAC with 10pF load)
    4. [5-bit DAC with 10k load](#5-bit DAC with 10k load)
5. [Layout](#paragraph3)
    1. [R_Divider](#R_Divider)
    2. [5-bit DAC](#5-bit DAC)
5. [Testing 5-bit DAC at different voltages](#paragraph4)
    1. [5-bit DAC with load](#5-bit DAC with load)
## Introduction <a name="introduction"></a>
1. The objective of the DAC was to initially use the R_Divider schematic for a portion of the 5-bit DAC and then use that to implement the 5-bit DAC. The 5-bit DAC is simulated on LTSpice and created on ElectricVLSI to observe and simulate a simple DAC. This simple 5-bit DAC will be implemented in future labs.

## Hand Calculations <a name="HandCalculations"></a>
The hand calculations needed were the output resistance, the delay with the 10pF capacitor, and the 10k load resistance DAC. The output resistance, delay with the 10pF load, and the 10k load resistance are shown in the figures in the subheaders below.

### Output Resistance <a name="OutputResistance"></a>
The output resistance calculation of the 5-bit DAC when all the inputs are grounded and the DAC does not have any capacitor or resistor load is 10kΩ and is shown in Figure 1 below.

![Output Resistance for DAC](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/86b7a7d6-bf25-4649-9bf1-e70af1053feb)

**Figure 1:** Calculation of the 5-bit DAC for output resistance
### delay with the 10pF capacitator load <a name="delay with the 10pF capacitator load"></a>
1. The delay of the 5-bit DAC with a 10pF capacitator load is calculated by delay = 0.7 * (10 * 10^3) * (10 * 10^-12) = 70ns as shown in Figure 2 below.

![handcalculations for load and delay](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/7edaf89c-9448-4648-b8bb-cf34e3ca3beb)

**Figure 2:** Calculation of the 5-bit DAC for delay

### Load of 10k resistor DAC <a name="Load of 10k resistor DAC"></a>
1. The effect of the load of 10k resistor on the DAC is calculated by doing the Thevenin theorem at the input voltage as 2V and applied ohm's law to get 100UA which is what I got for the simulation as well and it is shown in Figure 3 below.

![handcalculations for load and delay](https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/4f9661e8-d13c-46bc-b82d-f55c62ba2e96)


**Figure 3:** Calculation of the 5-bit DAC with 10k load resistor

## Schematics <a name="Schematics"></a>
1. These section covers the Schematics and the respective simulations of the R_Divider, the 5-bit DAC, 5 bit DAC with 10pF load, and 5 bit DAC with 10k load.

### R_Divider <a name="R_Divider"></a>
1. The schematic of the R_Divider is shown in Figure 4 and the simulation values are shown in Figure 5 below.

<img width="847" alt="R_Divider schematic" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/39b8d321-3a68-4313-9c14-69979ec0c42a">

**Figure 4:** Schematic of the R_Divider

<img width="470" alt="R_divider simulation results" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/693b1fd0-4bec-49c3-b77e-de903b4bef87">

**Figure 5:** Simulation of R_Divider on LTSpice


### 5-bit DAC <a name="5-bit DAC"></a>
1. The schematic of the 5-bit DAC is shown in Figure 6 and the simulation values are shown in Figure 7 below.

<img width="637" alt="5 bit DAC without load" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/332c167d-fed4-4d19-b4ad-59e0f15b6bdf">

**Figure 6:** Schematic of 5-bit DAC

<img width="698" alt="simulation values of layout of DAC without resistor load" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/e721c6b1-eca1-4cdb-9489-901535eafdbb">

**Figure 7:** Simulation of 5-bit DAC on LTSpice

### 5-bit DAC with 10pF load <a name="5-bit DAC with 10pF load"></a>
1. The schematic of the 5-bit DAC with 10pF is shown in Figure 8 and the simulation values are shown in Figure 9 below.

<img width="679" alt="5 bit DAC with capacitator load" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/5efc9efd-6646-48bf-9b7d-9ad72f37e386">

**Figure 8:** Schematic of 5-bit DAC with 10pF load at 2V

<img width="1277" alt="LT Spice for capacitator 2v DAC" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/b89e5db1-9f2e-448e-8385-fcbcb59891bd">

**Figure 8:** Simulation of 5-bit DAC with 10pF load at 2V

### 5-bit DAC with 10k load <a name="5-bit DAC with 10k load"></a>
1. The schematic of the 5-bit DAC with 10k is shown in Figure 10 and the simulation values are shown in Figure 11 below.
<img width="587" alt="DAC with resistor load schematic" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/bf8a64d0-050a-4543-b12d-4d25b9406eae">

**Figure 10:** Schematic of 5-bit DAC with 10k load at 2V

<img width="1273" alt="voltage simulation with resistor load for 2v" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/0b14038e-b087-486c-9571-22cc6b066e03">

**Figure 11:** Simulation of 5-bit DAC with 10k load at 2V

## Layout <a name="Layout"></a>
1. These section covers the Layouts of the R_Divider, and the entire 5-bit DAC with the load capacitator and resistor.

### R_Divider <a name="R_Divider"></a>
1. The layout of the R_Divider is shown in Figure 12 below.

<img width="654" alt="layout of R_Divider" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/3fc8a1dc-7e10-49fc-b78a-a1e241e402a5">

**Figure 12:** Layout of the R_Divider

### 5-bit DAC <a name="5-bit DAC"></a>
1. The layout of the 5-bit DAC is shown in Figure 13 below.

<img width="644" alt="DAC" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/4fdf22f8-fb71-41d8-98e6-b63a412514ab">


**Figure 13:** Layout of the 5-bit DAC
## Testing 5-bit DAC at different voltages <a name="Testing 5-bit DAC at different voltages"></a>
1. These show the Simulations of the 5-bit DAC with either a 10k resistor or 10pF capacitator at different voltages in the figures below.

### 5-bit DAC with load <a name="5-bit DAC with load"></a>
1. The simulation of DAC with load at 1v is shown in Figure 14, DAC with load at 3V is shown in Figure 15, and DAC with load at 4V is shown at FIgure 16 all shown below.

<img width="1277" alt="simulation of DAC with load at 1V" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/7ae887b9-24bc-46d0-a8f4-e73ee2caa266">

**Figure 14:** Schematic of 5-bit DAC with load at 1V

<img width="1267" alt="simulation with resistor load at 3V" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/37ef3853-1135-40c7-84bf-4ab6b26ae310">

**Figure 15:** Schematic of 5-bit DAC with load at 3V

<img width="1277" alt="DAC with load for 4V" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/eab3074e-6acd-44d7-8bdb-9cf94d7e3d9e">

**Figure 16:** Schematic of 5-bit DAC with load at 4V

<img width="849" alt="error analysis" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/dc0f284c-d931-4286-931d-0b1e349122e3">

**Figure 17:** Schematic of 5-bit DAC with load at 4V



<img width="850" alt="NCC analysis" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/caddfdcc-ab50-47df-9674-133a8808b8be">

**Figure 18:** Schematic of 5-bit DAC with load at 4V
















   










 
