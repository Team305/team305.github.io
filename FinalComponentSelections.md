---
title: Final Component Selection
---

# 6.0 Final Component Selection
Team 305 chose the following components for use in the weather monitoring project. Pros, Cons, and rationale for each component is found here. For additional information on the selection processes, as well as a comparison between all components considered, please refer to [Appendix B: Component Selection](/AppendixB) and [Appendix C: Microcontroller Selection](/AppendixC)
## 6.1 Final Components

### Temperature Sensor
 
|                                         Solution                                        |                                                                          Pros                                                                          |                                                Cons                                                |
|:---------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------:|
| ![1](/photos/Figure6a.png) <br>TC74A4-3.3VCTTR surface mount temp sensor <br>$1.09/each  <br>[Link Here](https://www.digikey.com/en/products/detail/microchip-technology/TC74A4-3-3VCTTR/443268) |           -Digital Sensor Wide supple range 2.7v~5.5v <br>-Low Power 200µA operating current <br>-Thermistor Replacement <br>-I2C compatible           |                          -No SPI compatibility <br>-No UART compatibility                          |

#### Chosen Component: TC74A4-3.3VCTTR
This sensor checks off all the necessary requirements needed for a temperature sensor. It is a digital sensor, I2C compatible, and it runs off low power. Team 305 must attempt to use as little power as possible when choosing components. This sensor is also available to Team 305 as a through hole component, which allows for testing before PCB design.

### Light Sensor

|                           Solution                           |                                                                                     Pros                                                                                    |                                                                                                                          Cons                                                                                                                          |
|:------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| ![1](/photos/Figure6d.png) <br>AS7343 L-DLGM <br>$11.11/each <br>[Link Here](https://www.digikey.com/en/products/detail/ams-osram/AS7343L-DLGM/16724750)  | -Has 1.8V supply voltage <br>-Can read 380 nm to 1000 nm wavelengths <br>-12C compatible  <br>-13 channels, one for each wavelength                                         | -Very small dimensions, ~3 mm long<br>-Bottom solder pads, will need to use solder paste<br>-Relatively expensive for one sensor                                                                                                                       |

#### Chosen Component: AS7343L-DLGM
This light sensor is the best choice for Team 305 - mainly for broad spectrum capabilities, supply voltage range, and method of communication (I2C). The data sheet is very descriptive and provides users with application notes, detailed diagrams, code examples, detailed pin readout, and lots of other well documented information that is pertinent to Team 305’s application. While it does have considerably small dimensions, it was one of the only sensors that fit all the needs of Team 305. For these reasons Team 305 feels that Option 1 will suffice to meet project requirements. 

### Motor Controller 

|                        Solution                        |                                                                            Pros                                                                            |                                                  Cons                                                  |
|:------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------:|
| ![1](/photos/Figure6g.png) <br>IFX9201SGAUMA1 <br>$4.88 <br>[Link Here](https://www.digikey.com/en/products/detail/infineon-technologies/IFX9201SGAUMA1/5415542) | -One used in class so programming is easier <br>-Supply voltage and output are all within the range needed <br>-Lots of documentation <br>-Up to 6A output | -Limited on motors that are compatible with this device <br>-Limited to only SPI and PWM communication |

#### Chosen Component: IFX9201SGAUMA1
For the motor controller, the optimal solution found was the IFX9201SGAUMA1. This is because it is the controller that was provided in class, and it allows for all the key features needed from this part. Its ability to be powered by a 3V supply is also a huge advantage compared to the other controllers. Overall this option is the best choice.

### Motor

|                                    Solution                                    |                                                                                                                Pros                                                                                                               |                                                                                         Cons                                                                                        |
|:------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| ![1](/photos/Figure6j.png) <br>1568-ROB-15277-ND SparkFun Electronics <br>$6.88 <br>[Link Here](https://www.digikey.com/en/products/detail/sparkfun-electronics/ROB-15277/9995750) | -Geared motor allowing for more torque <br>-6-24V input range allowing for it to operate within low and high voltage  <br>-Lightweight  Product                                                                                   | -Above logic level voltage <br>-Very low RPM 200                                                                                                                                    |

#### Chosen Component: 1568-ROB-15277-ND SparkFun Electronics
The best component found for the motor was the 1568-ROB-15277-ND from SparkFun Electronics. This high torque motor allows the project's moving parts to translate efficiently. This is a very cost effective motor that has a wealth of information scattered across the web in case there is any need for assistance. The gearbox inside allows for slow and precise movement of objects that have some weight to them. Overall, with its ability to be powered by the 9V main supply and high torque for its cost and size, this motor is the best option. 

### Linear + Switching Regulator

|                            Solution                           |                                                      Pros                                                      |                                                Cons                                               |
|:-------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------:|
| ![3](/photos/Figure6o.png) <br>LM2575S-3.3/NOPB <br>$4.90/each <br>[Link Here](https://www.mouser.com/ProductDetail/Texas-Instruments/LM2575S-3.3-NOPB?qs=X1J7HmVL2ZGH5uY2hHZLXw%3D%3D) | -Tested by Team 305 previously in class<br>-Desired output current <br>-Can output 3.3v                        | -Relatively high cost High demand <br>-Package is different from what Team 305 is used to.        |

#### Chosen Component: LM2575S-3.3/NOPB
The LM2575S-3.3/NOPB is the ideal choice for Team 305 because of its ease of use, high stock at Mouser, and non-excessive features. Compared to the other options we explored, this regulator does not have extraneous features that Team 305 does not plan to use. Additionally - this regulator has the desired current and voltage output to power the PIC MCU (3.3 V) and the motor chosen above. 

### AC-DC Wall adapter

|                         Solution                         |                                                                  Pros                                                                 |                             Cons                            |
|:--------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------:|
| ![3](/photos/Figure6r.png) <br>B09YRGM86T <br>$4.39/each <br>[Link Here](https://www.amazon.com/Aclorol-100V-240V-5-5mmX2-5mm-Elliptical-Security/dp/B09YRGM86T/ref=sr_1_5?gclid=Cj0KCQiAorKfBhC0ARIsAHDzsltCRRGZa2Ene-E88G765J7y5mwNfMPp0PXX9cqmOCVH6r3tmDEA8TEaAn1sEALw_wcB&hvadid=173531645013&hvdev=c&hvlocphy=9030087&hvnetw=g&hvqmt=e&hvrand=3654037398574692265&hvtargid=kwd-10120937855&hydadcr=19108_9439007&keywords=9v+1a+power+supply&qid=1676511133&sr=8-5)  | -Desired output voltage for motors to be functional <br>-Can output 9V <br>-Works within voltage regulators range.                    | -Can only output 1A <br>-No overload protection<br>         |

#### Chosen Component: B09YRGM86T
The B09YRGM86T is the ideal choice for Team 305 because of its lower cost and ability to power all necessary systems effectively. The other options are either too high or low in current and voltage output making the choice clear. This wall jack is also the most cost effective allowing for the team to spend money elsewhere.  

### Microcontroller

|                         Solution                         |                                                                  Pros                                                                 |                             Cons                            |
|:--------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------:|
| ![3](/photos/MicrocontrollerPIC18.png) <br>PIC18LF67K40 <br>$/each <br>[Link Here](https://www.mouser.com/ProductDetail/Microchip-Technology/PIC18LF67K40-I-PT?qs=Cv1v43EOJpoXOD%2FmCo0jeQ%3D%3D)  | -Can operate at 3.3V<br>-64 pins for additional purposes                    | -8-bit Microcontroller<br>-Max ADC Resolution = 10         |

#### Chosen Component: PIC18LF67K40
The PIC18LF67K40, despite its relatively low ADC resolution, is the best choice for the project. The amount of pins that the IC has as well as the multitude of packages available make the PIC18F67K40 the ideal component due to its flexibility and adaptability.

### Level Translator

|                         Solution                         |                                                                  Pros                                                                 |                             Cons                            |
|:--------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------:|
| ![3](/photos/level.jpg) <br>NVT2003 <br>$0.91/each <br>[Link Here](https://www.mouser.com/ProductDetail/NXP-Semiconductors/NVT2003DP118?qs=vbj%2FKoHZRAiMv2YX75DayA%3D%3D)  | <br>                    | <br><br>         |

#### Chosen Component: NVT2003
The NVT2003 a voltage translator used to convert the 1.8V outped by the light sensor to the systems logic level of 3.3V. This is a low cost surface mount chip fits all the requirements needed for the light sensors design.  

### Low-Dropout Regulator (LDO)

|                         Solution                         |                                                                  Pros                                                                 |                             Cons                            |
|:--------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------:|
| ![3](/photos/ldo.jpg) <br>ADP151 <br>$1.60/each <br>[Link Here](https://www.mouser.com/ProductDetail/Analog-Devices/ADP151AUJZ-1.8-R7?qs=sGAEpiMZZMutXGli8Ay4kD%2F4TpDpCbliGE0vLEUhOvE%3D)  | -<br>-<br>-                    | -<br>-<br>         |

#### Chosen Component: ADP151
The ADP151 is a 3.3-1.8V linear voltage regulator. This chip is the optimal choice for team 305 as it is surface mount and allows for voltage requirements of light sensors to be met.   


## 6.2 Generated Power Budget
![Figure 6z PowerBill](/photos/PowerBudget.png "Generated Power Bill")



[click here to return to index](/index)
