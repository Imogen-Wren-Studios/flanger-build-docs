# flanger-build-docs
Build docs for Imogen Wren Studios (Formally PGFX) BBD Dual Mode Analog Flanger

## PCB Layout
![image](https://user-images.githubusercontent.com/97303986/219202178-a9339f74-8108-4576-b86b-af8f09a7280c.png)


## Build Notes: Please read entire document before commencing build!
_We Recommend starting with the smallest components first, the resistors and diodes, before moving onto
sockets for the ICs, caps and transistors._ **Check the polarity of diodes and Electrolytic caps!**

---
### NOTES REGARDING BBD CHIP SELECTION

This PCB has been designed to work with MN3207/8 BBDs and MN3102 Clocks. You can mix and match
between MN3207s and MN3208 chips if desired. MN3208 has a slightly longer delay time so using this in
parallel with the MN3207 can create a deeper warble.

---

Before breaking apart the Footswitch Daughterboards, we find it easiest to connect the In, +, - and Out
with short runs of multi strand cable between the Main Board and the Bypass boards. <br>

This board is a neat true bypass solution, but can be omitted, just follow the labelling on the main board if
you wish to implement your own bypass circuit. <br>

The other footswitch daughterboard switches in the 2nd BBD delay line to effectively double the intensity
of the flanging effect. All the connections on this board need to be connected with the pin’s opposite on
the main board. It is easiest to do this before breaking them apart. The daughterboard can be replaced
with a SPST toggle switch if a second footswitch is undesired. The switch should connect and break the
Lsnd and Lrtn on the main board <br>

The Trim pot on the Daughterboards are for LED Brightness. We tend to use between 50-100k but you can omit it
entirely, just short either of the 2 pins that are already connected together to the 3rd pin. <br>

Once the top side of the board is populated, the Pots can be placed as well as the bypass footswitch, we
recommend soldering a single pin of each, aligning the PCB in the enclosure and then soldering the rest of
the pins. This ensures the PCB is fitted neatly and there is no undue stress on any of the connections.
Before the PCB is mounted in the box, we also find it easiest to solder some long flying leads for the Jacks
and DC Connections to the Bypass Daughterboard. <br>

The Ji – Jack in, and Jo – Jack out pins, as well as the Ground wires for the jacks, and the Vin and GND to
the DC Jack should be soldered with multi stranded wire 10-15cm long that can be cut to length once
installed. <br>

The final components to solder to the board are the indication LEDs, our best practice is to solder the short
negative pin first, almost flush with the PCB, and leave the other pin unsoldered until it is lined up with the
hole in the enclosure. We use a 5mm LED bezel, but you can just drill the correct sized hole in the
enclosure and mount it direct. <br>

Install the board, attach all the hardware and then make sure the LED is sat correctly before soldering the
final pin. <br>

Now the offboard wiring can be completed to the In and Out jacks, and the DC Jack.  <br><br>

## Calibration - DO NOT SKIP THIS STEP!

_Once assembled you will need to set the trim pot for the correct operation._ <br>
Adjust the 100k TrimPot on the main board until the flanging effect is at its maximum, if you are hearing
distortion on the wet signal it is likely that this TrimPot needs adjustment.

## Mods
Some potential for mods are documented on the schematic below. A higher res PDF is available in this repo.

## Notes on Boxing & Drilling
This PCB is designed for Tall 4S1590BBT / 1590BBT or 1590C Enclosures. You may struggle to find room for
the jacks in a smaller enclosure.

No Drill template has been provided, but the PCB itself provides centre holes to line up drill marks. In the
case of the alpha pots, the 2 large mounting Pads and the pin 2 Pad can be used to align the drill marks.
It is easiest to do this before soldering the board.

## Schematic
Please see - [flanger-schematic](https://github.com/Imogen-Wren-Studios/flanger-build-docs/blob/main/flanger-schematic.pdf) for high res PDF
<img width="1255" alt="image" src="https://user-images.githubusercontent.com/97303986/219211411-5e52ded7-477c-44b4-8c36-12105310cc43.png">






## BOM

| BOM:              |  Value                           |  Type                                     |    Notes                                     |
| ----------------- | -------------------------------- | ----------------------------------------- | -------------------------------------------- |
| ---               | ---                              |  ---                                      |  ---                                         |
| Resistors         |                                  |                                           |                                              |
| R1                |  1k                              |  Resistor                                 |                                              |
| R2                |  10k                             |  Resistor                                 |                                              |
| R3                | 10k                              |  Resistor                                 |                                              |
| R4                |  10k                             |  Resistor                                 |                                              |
| R5                |  4k7                             |  Resistor                                 |                                              |
| R6                |  10k                             |  Resistor                                 |                                              |
| R7                |  22k                             |  Resistor                                 |                                              |
| R8                |  1k                              |  Resistor                                 |                                              |
| R9                |  56k                             |  Resistor                                 |                                              |
| R10               |  330k                            |  Resistor                                 |                                              |
| R11               |  10k                             |  Resistor                                 |                                              |
| R12               |  470k                            |  Resistor                                 |                                              |
| R13               |  470k                            |  Resistor                                 |                                              |
| R14               | 100k                             |  Resistor                                 |                                              |
| R15               | 10k                              |  Resistor                                 |                                              |
| R16               | 10k                              |  Resistor                                 |                                              |
| R17               | 10k                              |  Resistor                                 |                                              |
| R18               | 10k                              |  Resistor                                 |                                              |
| R19               | 100k                             |  Resistor                                 |                                              |
| R20               | 22k                              |  Resistor                                 |                                              |
| R21               | 10k                              |  Resistor                                 |                                              |
| R22               | 56k                              |  Resistor                                 |                                              |
| R23               | 330k                             |  Resistor                                 |                                              |
| R24               | 220k                             |  Resistor                                 |                                              |
| R25               | 2k2-4k7 For High Brightness LED  |  CLR Resistor                             |                                              |
| R26               |  100k                            |  Resistor                                 |                                              |
| R27               |  330k                            |  Resistor                                 |                                              |
| R28               |  33k                             |  Resistor                                 |                                              |
| R29               |  470k                            |  Resistor                                 |                                              |
| R30               |  1k                              |  Resistor                                 |                                              |
| R31               |  2k2                             |  Resistor                                 |                                              |
| R32               |  4k7                             |  Resistor                                 |                                              |
| R33               |  1k                              |  Resistor                                 |                                              |
| R34               |  4k7                             |  Resistor                                 |                                              |
| R35               |  4k7                             |  Resistor                                 |                                              |
| R36               |  100k                            |  Resistor                                 |                                              |
| R37               |  100k                            |  Resistor                                 |                                              |
| R38               |  10k                             |  Resistor                                 |                                              |
| R39               |  220k                            |  Resistor                                 |                                              |
| R40               |  10k                             |  Resistor                                 |                                              |
| R41               |  33k                             |  Resistor                                 |                                              |
| R42               |  150k                            |  Resistor                                 |                                              |
| R43               |  68k                             | Resistor                                  |                                              |
| R44               |  470k                            |  Resistor                                 |                                              |
| R45               |  4k7                             |  Resistor                                 |                                              |
| R46               |  10k                             |  Resistor                                 |                                              |
| R47               |  10k                             |  Resistor                                 |                                              |
| R48               |  2k2-4k7 For High Brightness LED | CLR Resistor                              |                                              |
| R49               |  22r                             |  Resistor                                 |                                              |
| R50               |  10k                             |  Resistor                                 |                                              |
| R51               |  10k                             |  Resistor                                 |                                              |
| Rdry1             |  33k                             |  Resistor                                 |  Dry Signal Level                            |
| Rfb1              |  1k                              |  Resistor                                 |  Feedback Signal Level                       |
| Rl1               |  27k                             |  Resistor                                 |  Output Level                                |
| ---               | ---                              |  ---                                      |  ---                                         |
| Caps              |                                  |                                           |                                              |
| C1                |  100n                            |  FilmCapacitor Wima                       |                                              |
| C2                |  100n                            |  FilmCapacitor Wima                       |                                              |
| C3                |  10n                             |  FilmCapacitor                            |                                              |
| C4                |  470p                            |  FilmCapacitor                            |                                              |
| C5                | Builders Choice.                 |  FilmCapacitor                            |  Creates Lowpass filter in the feedback line |
| C6                |  33n                             |  FilmCapacitor                            |                                              |
| C7                |  100n                            |  FilmCapacitor Wima                       |                                              |
| C8                |  33n                             |  FilmCapacitor                            |                                              |
| C9                |  100p                            |  FilmCapacitor                            |                                              |
| C10               |  1n                              |  FilmCapacitor                            |                                              |
| C11               |  4n7                             |  FilmCapacitor                            |                                              |
| C12               |  3n3                             |  FilmCapacitor                            |                                              |
| C13               | 3n3                              |  FilmCapacitor                            |                                              |
| C14               |  33n                             |  FilmCapacitor                            |                                              |
| C15               |  100n                            |  FilmCapacitor Wima                       |                                              |
| C16               |  2n2                             |  FilmCapacitor                            |                                              |
| C17               |  1u                              |  FilmCapacitor                            |                                              |
| C18               |  10n                             |  FilmCapacitor                            |                                              |
| C19               |  4p7                             |  FilmCapacitor                            |                                              |
| C20               |  47p                             |  FilmCapacitor                            |                                              |
| ---               | ---                              |  ---                                      |  ---                                         |
| Electrolytic Caps |                                  |                                           |                                              |
| EC1               |  1u                              |  ElectrolyticCapacitor                    |                                              |
| EC2               |  10u                             |  ElectrolyticCapacitor                    |                                              |
| EC3               |  1u                              |  ElectrolyticCapacitor                    |                                              |
| EC4               |  22u                             |  ElectrolyticCapacitor                    |                                              |
| EC5               |  22u                             |  ElectrolyticCapacitor                    |                                              |
| EC6               |  10u                             |  ElectrolyticCapacitor                    |                                              |
| EC7               |  10u                             |  ElectrolyticCapacitor                    |                                              |
| EC8               |  10u                             |  ElectrolyticCapacitor                    |                                              |
| EC9               |  10u                             |  ElectrolyticCapacitor                    |                                              |
| EC10              |  10u                             |  ElectrolyticCapacitor                    |                                              |
| EC11              |  220u                            |  ElectrolyticCapacitor                    |                                              |
| EC12              |  100u                            |  ElectrolyticCapacitor                    |                                              |
| ---               | ---                              |  ---                                      |  ---                                         |
| Transistors       |                                  |                                           |                                              |
| Q1                |  2N5087                          |  transistors Small Signal PNP             |                                              |
| Q2                |  2N5088                          |  transistors Small Signal NPN             |                                              |
| Q3                |  2N5088                          |  transistors Small Signal NPN             |                                              |
| Q4                | 2N5088                           |  transistors Small Signal NPN             |                                              |
| ---               | ---                              |  ---                                      |  ---                                         |
| ICs               |                                  |                                           |                                              |
| IC1               | 4558                             |  integrated_circuits                      |  Dual Opamp                                  |
| IC2               |  MN3207_BBD                      |  integrated_circuits                      |  BBD                                         |
| IC3               |  MN3207/8_BBD                    |  integrated_circuits                      |  BBD                                         |
| IC4               |  4558 integrated_circuits        |  Dual Opamp                               |                                              |
| IC5               |  MN3102_CLK                      |  integrated_circuits                      |  BBD Clock                                   |
| IC6               |  TL022                           |  integrated_circuits                      |  Low Power Opamp                             |
| ---               | ---                              |  ---                                      |  ---                                         |
| Regulators        |                                  |                                           |                                              |
| REG1              |  L7805                           |  regulators                               |  +5v Regulator                               |
| Potentiometers    |                                  |                                           |                                              |
| Depth4            |  B50k                            |  Potentiometer 16mm Right Angle PCB Mount |                                              |
| Manual3           |  B50k                            |  Potentiometer 16mm Right Angle PCB Mount |                                              |
| Rate5             |  C500k                           | Potentiometer 16mm Right Angle PCB Mount  |                                              |
| Regen2            |  B50k                            |  Potentiometer 16mm Right Angle PCB Mount |                                              |
| Trim1             |  100k                            |  TrimPot BBD Bias Voltage                 |                                              |
| Trim2             |  LED TrimPot                     |  LED Brightness 50-100k                   |                                              |
| Trim3             |  LED TrimPot                     |  LED Brightness 50-100k                   |                                              |
| ---               | ---                              |  ---                                      |  ---                                         |
| Diodes            |                                  |                                           |                                              |
| D1                |  LEDA diodes                     |  Diodes:3MM_B                             |                                              |
| D2                |  1n4148 diodes                   |  Diodes:DO35-3                            |                                              |
| D3                |  1n4148 diodes                   |  Diodes:DO35-3                            |                                              |
| D4                |  LEDA diodes                     |  Diodes:3MM_B                             |                                              |
| D5                |  1n4148 diodes                   |  Diodes:DO35-3                            |                                              |
| D6                |  1n4007 diodes                   |  Diodes:DO41-3                            |                                              |
| ---               | ---                              |  ---                                      |  ---                                         |
| Switches          |                                  |                                           |                                              |
| SW1               |  3PDT                            |  Footswitch Switches:3PDT                 |                                              |
| SW2               |  3PDT                            |  Footswitch Switches:3PDT                 |                                              |

## Other Products from Imogen Wren Studios
![image](https://user-images.githubusercontent.com/97303986/219211201-3ce0cbd2-641a-4378-af77-50c6060aa029.png)

