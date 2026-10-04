# Guitar-Effects
For half life‘ onboard Guitar effects
<img width="591" height="438" alt="Screenshot 2026-10-01 144035" src="https://github.com/user-attachments/assets/cb759d29-65ce-4757-bb3c-c1c11d2907f2" />
First design on Distortion pedal based off this youtube Video https://www.youtube.com/watch?v=RXIqUyW2syU
 Basing it off a Boss DS1 Pedal with Mods
 schematic I have made for this pedal<img width="3301" height="2550" alt="Boss DS1 Mod(distortion change) (1) (1)-2" src="https://github.com/user-attachments/assets/a2f3289d-b511-48d0-93cb-f071dc29c8b1" />
<img width="3301" height="2550" alt="Boss DS1 Mod(distortion change) (1) (1)-1" src="https://github.com/user-attachments/assets/1e4d4691-24bb-4350-9463-065353095ba1" />

Part list so far  

[bom (1).csv](https://github.com/user-attachments/files/32946430/bom.1.csv)

Name,Quantity,Component
"3, 4, 5",3," Breadboard Small"
"BAT1",1," 9V Battery"
"R3, R4, Rr3, Rr18, Rr21, R11",6,"10 kΩ Resistor"
"C2",1,"47 uF Capacitor"
"PIEZO1, PIEZO2",2," Piezo"
"Rr1, R1, Rr22, R9",4,"1 kΩ Resistor"
"C1, Cc3",2,"47 nF Capacitor"
"Rr2, Rr7",2,"470 kΩ Resistor"
"Tq1, T2, T1",3," NPN Transistor (BJT)"
"Cc2, Cc8, Cc9",3,"0.47 uF Capacitor"
"Meter1, Meter2",2,"Voltage Multimeter"
"Rr4, Rr5, Rr10, Rr11, Rr23",5,"100 kΩ Resistor"
"Rr9",1,"22 Ω Resistor"
"Cc4",1,"250 pF Capacitor"
"Cc5",1,"68 nF Capacitor"
"Rr39",1,"47 kΩ Resistor"
"D1, D2, D3",3," Diode"
"U1, U2",2," 741 Operational Amplifier"
"Cc7",1,"100 pF Capacitor"
"Rpotvr11",1,"100 kΩ Potentiometer"
"Rr14",1,"1.5 kΩ Resistor"
"C3",1,"0.01 uF Capacitor"
"Cc11",1,"0.022 uF Capacitor"
"Rr15, R2",2,"2.2 kΩ Resistor"
"Rr16, Rr17",2,"6.8 kΩ Resistor"
"Cc12",1,"0.1 uF Capacitor"
"Rpot3, Rpot4",2,"250 kΩ Potentiometer"
"R6, R7",2,"1 mΩ Resistor"
"Cc13",1,"0.05 uF Capacitor"
"Cc14",1,"1 uF Capacitor"
"S1, S2, S3, S4, S5, S6",6," Slideswitch"
"R5, R10",2,"3.3 kΩ Resistor"
"R8",1,"4.7 kΩ Resistor"

The current file made on 3rd of October 2026, can only be used in LIVESPICE

<?xml version="1.0" encoding="utf-8"?>
<Schematic Name="X1" PartNumber="">
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-770,-45">
    <Component _Type="Circuit.Input, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" V0dBFS="1 V" Name="V1" Description="Ideal voltage source representing an input port." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-770,-15">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND1" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-770,-25" B="-770,-15" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-735,-70">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="1 kΩ" Name="R1" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-770,-70" B="-770,-65" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-770,-70" B="-755,-70" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-690,-70">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="47 nF" Name="C1" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-715,-70" B="-710,-70" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-660,-110">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="470 kΩ" Name="R2" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-630,-70">
    <Component _Type="Circuit.BipolarJunctionTransistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Type="NPN" IS="1 pA" BF="100" BR="1" Name="Q1" Description="" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-660,-90" B="-660,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-670,-70" B="-660,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-660,-70" B="-650,-70" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-620,-10">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="10 kΩ" Name="R3" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-620,-50" B="-620,-30" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-620,10" B="-620,15" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-620,15">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND2" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-700,-180">
    <Component _Type="Circuit.VoltageSource, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Voltage="4.5 V" Name="V4" Description="Ideal voltage source." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-660,-200" B="-660,-130" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-700,-160" B="-700,-155" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-700,-155">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND5" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-660,-245">
    <Component _Type="Circuit.VoltageSource, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Voltage="9 V" Name="V5" Description="Ideal voltage source." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-660,-225" B="-660,-220" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-660,-220">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND6" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-620,-265" B="-620,-90" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="true" Position="-585,-50">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="470 nF" Name="C2" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-620,-50" B="-605,-50" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-4" Flip="false" Position="-550,-95">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R4" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="true" Position="-515,-50">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="47 nF" Name="C3" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-550,-75" B="-550,-50" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-565,-50" B="-550,-50" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-550,-50" B="-535,-50" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-4" Flip="false" Position="-495,-10">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R5" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-495,-50" B="-495,-30" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-495,10" B="-495,15" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-495,15">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND7" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-440,-50">
    <Component _Type="Circuit.BipolarJunctionTransistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Type="NPN" IS="1 pA" BF="100" BR="1" Name="Q2" Description="" />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="true" Position="-440,-100">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="470 kΩ" Name="R6" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="true" Position="-440,-155">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="250 pF" Name="C4" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-495,-50" B="-460,-50" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-460,-155" B="-460,-100" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-460,-100" B="-460,-50" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-420,-100" B="-420,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-430,-70" B="-420,-70" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-2" Flip="false" Position="-430,20">
    <Component _Type="Circuit.SP4T, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Position="0" Group="" Name="S1" Description="single pole quadruple-throw switch." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-430,-30" B="-430,0" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-490,85">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="22 Ω" Name="R7" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-440,100">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="1 kΩ" Name="R8" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-420,145">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="3.3 kΩ" Name="R9" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-400,180">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="10 kΩ" Name="R10" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-490,40" B="-460,40" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-490,40" B="-490,65" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-440,40" B="-440,80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-420,40" B="-420,125" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-400,40" B="-400,160" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-400,210">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND9" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-490,105" B="-490,120" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-490,120" B="-440,120" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-440,120" B="-440,165" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-440,165" B="-420,165" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-420,165" B="-420,200" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-420,200" B="-400,200" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-400,200" B="-400,210" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-420,-210">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="10 kΩ" Name="R11" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-420,-190" B="-420,-155" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-420,-155" B="-420,-100" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-400,-70">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="65 nF" Name="C5" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-330,-95">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R12" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-265,-70">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="47 kΩ" Name="R39" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-380,-70" B="-330,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-330,-70" B="-285,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-330,-75" B="-330,-70" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="true" Position="-240,-30">
    <Component _Type="Circuit.Diode, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" IS="2.52 nA" n="1.752" Type="Diode" Name="D1" PartNumber="1N4148" Description="" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-240,-10" B="-240,0" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-240,0">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND12" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-245,-70" B="-240,-70" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-150,-80">
    <Component _Type="Circuit.OpAmp, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rin="2 MΩ" Rout="75 Ω" Aol="200 k" GBP="1 MHz" Name="X1" PartNumber="UA741" Description="Generic op-amp model. Model includes a single pole frequency response and saturation." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-130,-80" B="-90,-80" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="0,-80">
    <Component _Type="Circuit.OpAmp, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rin="2 MΩ" Rout="75 Ω" Aol="200 k" GBP="1 MHz" Name="X2" PartNumber="UA741" Description="Generic op-amp model. Model includes a single pole frequency response and saturation." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-90,-190" B="-90,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-90,-80" B="-90,-70" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="0,-195">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R13" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="65,-120">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="100 pF" Name="C7" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-65,-195" B="-20,-195" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="65,-195" B="65,-140" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="65,-100" B="65,-80" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-2" Flip="false" Position="110,-195">
    <Component _Type="Circuit.Potentiometer, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Wipe="0.5" Sweep="Linear" Group="" Name="R14" Description="Represents a potentiometer. When Wipe is 0, the wiper is at the cathode." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="20,-195" B="65,-195" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="65,-195" B="100,-195" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="120,-245" B="120,-215" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="120,-265">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="4.7 kΩ" Name="R15" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="120,-175" B="120,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="20,-80" B="65,-80" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="120,-310">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="470 nF" Name="C6" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="true" Position="120,-335">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND17" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="120,-335" B="120,-330" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="120,-290" B="120,-285" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="160,-80">
    <Component _Type="Circuit.SP4T, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Position="0" Group="" Name="S2" Description="single pole quadruple-throw switch." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="65,-80" B="120,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="120,-80" B="140,-80" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="210,-150">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="1.5 kΩ" Name="R16" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="210,-105">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="2.2 kΩ" Name="R17" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="210,-60">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="3.3 kΩ" Name="R18" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="210,-15">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="4.7 kΩ" Name="R19" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="180,-150" B="180,-110" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="180,-150" B="190,-150" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="190,-105" B="190,-90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="180,-90" B="190,-90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="180,-70" B="190,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="190,-70" B="190,-60" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="180,-50" B="190,-50" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="190,-50" B="190,-15" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="275,-80">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="470 nF" Name="C9" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="230,-150" B="255,-150" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="230,-105" B="230,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="230,-80" B="255,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="230,-60" B="255,-60" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="255,-150" B="255,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="230,-15" B="255,-15" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="255,-80" B="255,-60" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="255,-60" B="255,-15" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="true" Position="320,-115">
    <Component _Type="Circuit.Diode, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" IS="2.52 nA" n="1.752" Type="Diode" Name="D2" PartNumber="1N4148" Description="" />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="390,-115">
    <Component _Type="Circuit.Diode, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" IS="2.52 nA" n="1.752" Type="Diode" Name="D3" PartNumber="1N4148" Description="" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="320,-135" B="390,-135" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="355,-95" B="355,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="320,-95" B="355,-95" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="355,-95" B="390,-95" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="385,-60">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="10 nF" Name="C8" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="385,-30">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND19" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="385,-40" B="385,-30" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="295,-80" B="355,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="355,-80" B="385,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="500,-80" B="500,-60" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="500,-40">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="22 nF" Name="C10" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="500,20">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="2.2 kΩ" Name="R20" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="500,-20" B="500,0" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="595,-50">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="6.8 kΩ" Name="R21" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="645,-20">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="100 nF" Name="C11" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="665,-20" B="680,-20" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="680,-100" B="680,-20" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="595,-20" B="625,-20" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="595,-80" B="595,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="385,-80" B="500,-80" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="500,-80" B="595,-80" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="605,30">
    <Component _Type="Circuit.Potentiometer, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="20 kΩ" Wipe="0.5" Sweep="Linear" Group="" Name="R22" Description="Represents a potentiometer. When Wipe is 0, the wiper is at the cathode." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="595,-30" B="595,-20" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="595,-20" B="595,10" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="595,50" B="595,100" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="500,40" B="500,90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="500,90" B="595,90" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="595,120">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="6.8 kΩ" Name="R23" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="690,85">
    <Component _Type="Circuit.Potentiometer, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Wipe="0.5" Sweep="Linear" Group="" Name="R24" Description="Represents a potentiometer. When Wipe is 0, the wiper is at the cathode." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="640,135" B="640,130" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="615,30" B="680,30" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="680,30" B="680,65" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="735,85">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="10 kΩ" Name="R25" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="700,85" B="715,85" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="755,85" B="755,255" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-775,255" B="755,255" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-775,255" B="-775,625" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-665,625">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="47 nF" Name="C12" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-705,615" B="-705,625" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-775,625" B="-705,625" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-705,625" B="-685,625" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-600,615" B="-600,625" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-555,625">
    <Component _Type="Circuit.BipolarJunctionTransistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Type="NPN" IS="1 pA" BF="100" BR="1" Name="Q3" Description="" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-645,625" B="-600,625" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-600,625" B="-575,625" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-535,695">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="10 kΩ" Name="R28" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-475,655">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="1 kΩ" Name="R29" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-535,645" B="-535,675" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-545,645" B="-535,645" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-535,645" B="-495,645" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-495,645" B="-495,655" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-425,655">
    <Component _Type="Circuit.Capacitor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Capacitance="1 μF" Name="C13" Description="Standard capacitor component" />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-455,655" B="-445,655" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-535,715" B="-535,725" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-535,725">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND26" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-370,695">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R30" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-370,715" B="-370,725" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-370,725">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND27" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-405,655" B="-370,655" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-290,695">
    <Component _Type="Circuit.Speaker, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" V0dBFS="9 V" Impedance="∞ Ω" Name="S3" Description="Ideal speaker." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-290,670" B="-290,675" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-370,675" B="-290,675" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-370,630" B="-370,655" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-370,655" B="-370,675" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-175,-190">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R26" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-550,-200" B="-550,-115" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-420,-265" B="-420,-230" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-330,-200" B="-330,-115" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-150,-265" B="-150,-100" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-150,-265" B="0,-265" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="0,-265" B="0,-100" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-550,-200" B="-330,-200" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="320,-200" B="320,-135" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-330,-200" B="320,-200" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="320,-200" B="680,-200" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="680,-200" B="680,-100" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="595,140" B="680,140" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="680,105" B="680,140" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="565,-100" B="680,-100" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="565,-100" B="565,140" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="565,140" B="595,140" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-660,-265" B="-620,-265" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-620,-265" B="-420,-265" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-600,595">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R27" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-605,575" B="-600,575" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-575,535">
    <Component _Type="Circuit.VoltageSource, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Voltage="9 V" Name="V2" Description="Ideal voltage source." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-575,555" B="-575,560" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-575,560">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND3" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-575,515" B="-535,515" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-535,515" B="-535,605" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-545,605" B="-535,605" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-290,715" B="-290,720" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-290,720">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND4" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-700,-200" B="-660,-200" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-660,-200" B="-550,-200" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-190,-245">
    <Component _Type="Circuit.VoltageSource, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Voltage="9 V" Name="V3" Description="Ideal voltage source." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-190,-225" B="-190,-220" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-190,-220">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND8" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-190,-265" B="-150,-265" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-645,515">
    <Component _Type="Circuit.VoltageSource, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Voltage="4.5 V" Name="V6" Description="Ideal voltage source." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-645,535" B="-645,540" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-645,540">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND10" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-645,495" B="-600,495" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-600,495" B="-600,575" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-4" Flip="false" Position="0,-35">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND11" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="0,-60" B="0,-45" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="0,-45" B="0,-35" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-145,15">
    <Component _Type="Circuit.VoltageSource, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Voltage="4.5 V" Name="V7" Description="Ideal voltage source." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-145,35" B="-145,40" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-145,40">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND13" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-145,-5" B="-20,-5" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-65,-195" B="-65,-90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-215,-190" B="-215,-90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-180,-70" B="-180,-5" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-180,-5" B="-145,-5" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-155,-190" B="-90,-190" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-215,-190" B="-195,-190" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-150,-60" B="-150,-35" />
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="0" Flip="false" Position="-150,-35">
    <Component _Type="Circuit.Ground, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" WireName="GND" Name="GND14" Description="Nodes with the same name are connected as if they were connected by a continuous wire." />
  </Element>
  <Element Type="Circuit.Symbol, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Rotation="-1" Flip="false" Position="-60,-70">
    <Component _Type="Circuit.Resistor, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" Resistance="100 kΩ" Name="R31" Description="Standard resistor." />
  </Element>
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-40,-70" B="-35,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-90,-70" B="-80,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-20,-70" B="-20,-5" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-180,-70" B="-170,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-240,-90" B="-240,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-240,-70" B="-240,-50" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-240,-90" B="-215,-90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-215,-90" B="-170,-90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-35,-90" B="-35,-70" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-65,-90" B="-35,-90" />
  <Element Type="Circuit.Wire, Circuit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null" A="-35,-90" B="-20,-90" />
</Schematic>

New Build with 2 more gain or distortion options and a new option for bypass
<img width="1300" height="895" alt="Screenshot 2026-10-03 152819" src="https://github.com/user-attachments/assets/f2a7d4f1-3770-41e3-b759-54c73995fbaf" />

Final designs Schematic and breadboard

<img width="992" height="547" alt="Screenshot 2026-10-03 183823" src="https://github.com/user-attachments/assets/e0cd86e0-82c8-43ed-a083-b20723645dad" />
<img width="1259" height="908" alt="Screenshot 2026-10-03 134459" src="https://github.com/user-attachments/assets/100f5a27-2995-4f67-9a02-27b938c649bc" />
