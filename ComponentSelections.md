---
title: Component Selection
---

# 6.0 Component Selection

## Temperature Sensor
 
|                                         Solution                                        |                                                                          Pros                                                                          |                                                Cons                                                |
|:---------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------:|
| # Option 1. <br>TC74A4-3.3VCTTR surface mount temp sensor <br>$1.09/each  <br>Link here |           -Digital Sensor Wide supple range 2.7v~5.5v <br>-Low Power 200µA operating current <br>-Thermistor Replacement <br>-I2C compatible           |                          -No SPI compatibility <br>-No UART compatibility                          |
|     # Option 2. <br>TMP175AID surface mount temp sensor <br>$2.65/each <br>Link here    | -I2C compatible Wide supply range  2.7v~5.5v <br>-Temperature range of -40C to +125C <br>-Digital Sensor <br>-Small 8-Pin MSOP and 8-Pin SOIC Packages | -No SPI compatibility <br>-No UART compatibility<br>-Excessive features that would not be utilized |
|      # Option 3. <br>TMP75AID surface mount temp sensor <br>$1.44/each<br>Link here     |  -I2C compatible Wide supply range  2.7v~5.5v <br>-Temperature range of -40C to +125C<br>-Digital Sensor <br>-Small 8-Pin MSOP and 8-Pin SOIC Packages |                          -No SPI compatibility <br>-No UART compatibility                          |

### Optimal Solution: TC74A4-3.3VCTTR
When selecting a temperature sensor, Option 1 is best for Team 305. The reason for that is because it checks off all the necessary requirements needed for a temperature sensor. It is a digital sensor, I2C compatible, and it runs off low power. Team 305 must pay attention and use as little power as we can when choosing a component. Option 1 is also available to Team 305 as a through hole component, which allows us to test it before PCB design.

## Light Sensor

|                           Solution                           |                                                                                     Pros                                                                                    |                                                                                                                          Cons                                                                                                                          |
|:------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| # Option 1. <br>AS7343 L-DLGM <br>$11.11/each <br>Link here  | -Has 1.8V supply voltage <br>-Can read 380 nm to 1000 nm wavelengths <br>-12C compatible  <br>-13 channels, one for each wavelength                                         | -Very small dimensions, ~3 mm long<br>-Bottom solder pads, will need to use solder paste<br>-Relatively expensive for one sensor                                                                                                                       |
| # Option 2. <br>ADUX1020BCPZRL7 <br>$7.07/each <br>Link here | -Lower in cost <br>-Uses I2C communication <br>-Operates with the desired 1.8 V to 3.3V supply voltage range                                                                | -Smallest option compared to the other two sensors <br>-Has a limited light spectrum range <br>-Bottom solder leads                                                                                                                                    |
| # Option 3. <br>AS7343-DLGM <br>$12.10/each <br>Link here    | -Broad light spectrum range from 380 nm to 1000 nm <br>-I2C compatible <br>-Operates with desirable supply voltage 1.7V - 1.98 V <br>-14  channels, one for each wavelength | -Most expensive option compared to other two sensors <br>-Some of  the light within it’s sensor range is not relevant for agricultural applications  <br>-Small dimensions with bottom solder leads <br>-Most expensive option of the 3 sensor options |

### Optimal Solution: AS7343L-DLGM
Option 1 is the best choice for Team 305 - mainly for broad spectrum capabilities, supply voltage range, and method of communication (I2C). The data sheet is very descriptive and provides users with application notes, detailed diagrams, code examples, detailed pin readout, and lots of other well documented information that is pertinent to Team 305’s application. While it does have considerably small dimensions, it was one of the only sensors that fit all the needs of Team 305. Option 3 is almost the exact same chip - however Option 3 has an additional channel dedicated to a wavelength that Team 305 is not interested in measuring. For these reasons Team 305 feels that Option 1 will suffice to meet project requirements, which has less channels than Option 3. 

## Motor Controller 

|                        Solution                        |                                                                            Pros                                                                            |                                                  Cons                                                  |
|:------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------:|
| # Option 1. <br>IFX9201SGAUMA1 <br>$4.88 <br>Link here | -One used in class so programming is easier <br>-Supply voltage and output are all within the range needed <br>-Lots of documentation <br>-Up to 6A output | -Limited on motors that are compatible with this device <br>-Limited to only SPI and PWM communication |
| # Option 2. <br>NCV7544MWTXG <br>$4.21 <br>Link here   | -Fits requirements of part <br>-Can control multiple motors at once <br>-16-bit SPI                                                                        | -Limited to only SPI and PWM communication <br>-Required supply voltage over 3V                        |
| # Option 3. <br>TLE9201SGAUMA1 <br>$5.38 <br>Link here | -High operating temperature range<br>-Compatible with most DC motors <br>-Lots of documentation                                                            | -Required supply voltage over 3V <br>-Only works with one motor  <br>-Limited communication channels   |

### Optimal Solution: IFX9201SGAUMA1
For the motor controller the optimal solution is the IFX9201SGAUMA1. This is because it is the controller we will be working with in class and it allows for all the key features needed from this part. Its ability to be powered by a 3V supply is also a huge advantage compared to the other controllers. Overall this option is the best choice.

## Motor

|                                    Solution                                    |                                                                                                                Pros                                                                                                               |                                                                                         Cons                                                                                        |
|:------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| # Option 1. <br>1568-ROB-15277-ND SparkFun Electronics <br>$6.88 <br>Link here | -Geared motor allowing for more torque <br>-6-24V input range allowing for it to operate within low and high voltage  <br>-Lightweight  Product                                                                                   | -Above logic level voltage <br>-Very low RPM 200                                                                                                                                    |
| # Option 2. <br>3871 Adafruit Industries LLC. <br>$1.95 <br>Link here          | -Runs between 3-3.7V<br>-Meaning it will function with on board power <br>-Very small form factor allowing for easy placement within device  <br>-Unique design would allow for the sensors to easily be mounted on the  product. | -Not much power compared to the other options <br>-Low size means that it might wont be able to hold sensor <br>-Low power range means if there  is a voltage problem it could fail |
| # Option 3. <br>ROB-13258 <br>$5.50 <br>Link here                              | -High voltage input range from 3-6V<br>-Unique form factor allow for part to be placed in different areas easily <br>-High torque                                                                                                 | -Low RPM 65 <br>-High cost compared to other three options  <br>-All plastic internals                                                                                              |

### Optimal Solution: 1568-ROB-15277-ND SparkFun Electronics
The best component found for the motor was the 1568-ROB-15277-ND SparkFun Electronics. This high torque motor will allow for the movement aspect of our project to work efficiently. This is a very cost effective motor that has lots of information scattered across the web in case there is any need for assistance. The gear box inside allows for slow and precise movement of objects that have some weight to them. Overall with its ability to be powered by the 9V main supply and high torque for cost and size this motor is the best option. 

## Linear + Switching Regulator

|                            Solution                           |                                                      Pros                                                      |                                                Cons                                               |
|:-------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------:|
| # Option 1. <br>MAX14750CEWA+T<br>$4.63 <br>Link here         | -Has the desired output voltage <br>-Surface mount configuration <br>-Reasonable cost                          | -Has excessive features  <br>-Very small compared to the other options <br>-Untested by our group |
| # Option 2. <br>BD933N1WG-CTR <br>$1.34<br>Link here          | -Simple output <br>-No excessive features <br>-Very reasonable price <br>-Chisel tip leads  <br>-Surface mount | -Untested by Team 305 Minimum <br>-4.5V input                                                     |
| # Option 3. <br>LM2575S-3.3/NOPB <br>$4.90/each <br>Link here | -Tested by Team 305 previously in class<br>-Desired output current <br>-Can output 3.3v                        | -Relatively high cost High demand <br>-Package is different from what Team 305 is used to.        |

### Optimal Solution: LM2575S-3.3/NOPB
The LM2575S-3.3/NOPB is the ideal choice for Team 305 because of its ease of use, high stock at Mouser, and non-excessive features. Compared to the other options, Option 3 does not have features that Team 305 does not plan to use. Additionally - Option 3 has the desired current and voltage output to power the PIC MCU (3.3 V) and the motor chosen above. 

## AC-DC Wall adapter

|                         Solution                         |                                                                  Pros                                                                 |                             Cons                            |
|:--------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------:|
| # Option 1. <br>4336304932 <br>$12.99/each <br>Link here | -Has the output voltage within motors range <br>-12V+ High value <br>–Comes with 2 wall plugs Reasonable cost                         | -Very high Voltage <br>-2 A output  <br>-Cost is high       |
| # Option 2. <br>B09TQLNNSR <br>$13.99/each <br>Link here | -Simple output <br>-No excessive features <br>-Multiple tips for different barrel jack styles <br>-Low voltage allows for less danger | -Untested by Team 305 <br>-Max 5 V output <br>-Cost is high |
| # Option 3. <br>B09YRGM86T <br>$4.39/each <br>Link here  | -Desired output voltage for motors to be functional <br>-Can output 9V <br>-Works within voltage regulators range.                    | -Can only output 1A <br>-No overload protection<br>         |

### Optimal Solution: B09YRGM86T
The B09YRGM86T is the ideal choice for Team 305 because of its lower cost and ability to power all necessary systems effectively. The other options are either too high or low in current and voltage output making the choice clear. Option 3 is also the most cost effective allowing for the team to spend money elsewhere.  


## Generated Power Budget
![Figure XA PowerBill](/photos/PowerBudget.jpg "Generated Power Bill")

[click here to return to index](/index)
