# Lab # 3 - Nmos IC with ESD
# Table of contents
1. [Introduction](#introduction)
2. [Schematics](#paragraph1)
   
   1.[Nmos](#Nmos)
   
   2.[Final_IC_Not_ESD](#Final_IC_Not_ESD)
   
   3.[pActive_nWell] (#pActive_nWell)

   4.[pWell_nActive] (#pWell_nActive)
   
   5.[Pad_ESD] (#Pad_ESD)

   6.[Padframe_ESD] (#Padframe_ESD)

   7.[Final_IC_ESD](#Final_IC_ESD) 
4. [Layout](#paragraph3)


   1.[Nmos](#Nmos)
   
   2.[Final_IC_Not_ESD](#Final_IC_Not_ESD)
   
   3.[pActive_nWell] (#pActive_nWell)

   4.[pWell_nActive] (#pWell_nActive)
   
   5.[Pad_ESD] (#Pad_ESD)

   6.[Padframe_ESD] (#Padframe_ESD)

   7.[Final_IC_ESD](#Final_IC_ESD)
## Introduction <a name="introduction"></a>
    1. The objective of Lab 3 was to create a final ic with ESD protection using the pad and the padframe from tutorial 2 done in class and the Nmos from tutorial 3. The reason why ESD protection is necessary is because so that we can protect the electronic components and the IC from being damaged.
## Schematics <a name="Schematics"></a>
   1. This section covers the schematics of the Nmos, Final_IC_Not_ESD, pActive_nWell, pWell_nActive, Pad_ESD, Padframe_ESD, and Final_IC_ESD in the sub sections provided below.
## Nmos <a name="Nmos"></a>
   1. Figure 1 below shows the schematic of the Nmos that is a length of 2 and a width of 10 and shows the where the drain, gate, and source are located on the Nmos.
      
      <img width="686" alt="Nmos_IV" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/1a478170-3ce0-4ecc-bbfa-7b62185e8155">

      Figure 1: Schematic of NMOS
## Final_IC_Not_ESD <a name="Final_IC_Not_ESD"></a>
   1. Figure 2 below shows the schematic of the Final IC without the ESD protection and shows the Nmos schematic wired to the respective pins on the padframe in the layout and the Padframe schematic showing how many pins are on the padframe.
      <img width="834" alt="final_ic_notesd" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/d3a777aa-2540-45b4-bef9-3235d7247a91">

      Figure 2: Schematic of Final_IC_Not_ESD composed of NMOS and Padframe schematics
## pActive_nWell <a name="pActive_nWell"></a>
   1. Figure 3 below shows the schematic of pActive_nWell as a diode circuit and labels which side is the pActive and which side is the nWell.
      <img width="769" alt="pActive_nWell" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/2a4f4b39-0730-4501-b9db-d2140e1d734a">

      Figure 3: Schematic of pActive_nWell
## pWell_nActive <a name="pWell_nActive"></a>
   1. Figure 4 below shows the schematic of the pWell_nActive as a diode circuit and labels which side is the pWell and which side is the nActive.
      <img width="824" alt="pWell_nActive" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/e0f4861a-1117-4705-82fe-16e33679fff5">

      Figure 4: Schematic of pWell_nActive
## Pad_ESD <a name="Pad_ESD"></a>
   1. Figure 5 below shows the schematic of the Pad with ESD created with two diode circuits which are the pActive_nWell and the pWell_nActive wired with a VDD, inout, and gnd.
      <img width="642" alt="pad_esd" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/d6087bba-fe16-4b93-9497-cc85f577dc3e">

      Figure 5: Schematic of Pad with ESD
## Padframe_ESD <a name="Padframe_ESD"></a>
   1. Figure 6 below shows the schematic of the padframe with ESD created from the Pad_ESD schematic connected with pin[1:8], vdd, and gnd.
      <img width="795" alt="padframe_esd" src="https://github.com/Kkihamin/ENCE_3501_Projects/assets/129350322/7f0d326c-e6d8-471c-a6dd-2509c97b13cf">

      Figure 6: Schematic of Padframe_ESD composed from Pad_ESD schematic
      









 
