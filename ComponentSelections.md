# Component Selection

## Temperature Sensor

|                                          Solution                                         |                                                                  Pros                                                                 |                                           Cons                                           |
|:-----------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------:|
|        # Option 1. TC74A4-3.3VCTTR surface mount temp sensor $1.09/each  Link here        |           Digital Sensor Wide supple range 2.7v~5.5v Low Power 200µA operating current Thermistor Replacement I2C compatible          |                        No SPI compatibility No UART compatibility                        |
| # Option 2. TMP175AID surface mount temp sensor $2.65/each Link here                      | I2C compatible Wide supple range 2.7v~5.5v Temperature range of -40C to +125C Digital Sensor Small 8-Pin MSOP and 8-Pin SOIC Packages | No SPI compatibility No UART compatibility Excessive features that would not be utilized |
| # Option 3. TMP75AID surface mount temp sensor $1.44/each                       Link here | I2C compatible Wide supple range 2.7v~5.5v Temperature range of -40C to +125C Digital Sensor Small 8-Pin MSOP and 8-Pin SOIC Packages | No SPI compatibility No UART compatibility                                               |

### Optimal Solution: TC74A4-3.3VCTTR
When selecting a temperature sensor, Option 1 is best for Team 305. The reason for that is because it checks off all the necessary requirements needed for a temperature sensor. It is a digital sensor, I2C compatible, and it runs off low power. Team 305 must pay attention and use as little power as we can when choosing a component. Option 1 is also available to Team 305 as a through hole component, which allows us to test it before PCB design.

## Light Sensor

| Solution                                         | Pros                                                                                                                                                       | Cons                                                                                                                                                                                                                                  |
|--------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| # Option 1. AS7343 L-DLGM $11.11/each Link here  | Has 1.8V supply voltage Can read 380 nm to 1000 nm wavelengths 12C compatible  13 channels, one for each wavelength                                        | Very small dimensions, ~3 mm long Bottom solder pads, will need to use solder paste Relatively expensive for one sensor                                                                                                               |
| # Option 2. ADUX1020BCPZRL7 $7.07/each Link here | Lower in cost Uses I2C communication Operates with the desired 1.8 V to 3.3V supply voltage range                                                          | Smallest option compared to the other two sensors Has a limited light spectrum range Bottom solder leads                                                                                                                              |
| # Option 3. AS7343-DLGM $12.10/each Link here    | Broad light spectrum range from 380 nm to 1000 nm I2C compatible Operates with desirable supply voltage 1.7V - 1.98 V 14 channels, one for each wavelength | Most expensive option compared to other two sensors Some of the light within it's sensor range is not relevant for agricultural applications  Small dimensions with bottom solder leads Most expensive option of the 3 sensor options |

### Optimal Solution: AS7343L-DLGM
Option 1 is the best choice for Team 305 - mainly for broad spectrum capabilities, supply voltage range, and method of communication (I2C). The data sheet is very descriptive and provides users with application notes, detailed diagrams, code examples, detailed pin readout, and lots of other well documented information that is pertinent to Team 305’s application. While it does have considerably small dimensions, it was one of the only sensors that fit all the needs of Team 305. Option 3 is almost the exact same chip - however Option 3 has an additional channel dedicated to a wavelength that Team 305 is not interested in measuring. For these reasons Team 305 feels that Option 1 will suffice to meet project requirements, which has less channels than Option 3. 

## Motor Controller 

| Solution                                          | Pros                                                                                                                                        | Cons                                                                                             |
|---------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| # Option 1. IFX9201SGAUMA1 Price: $4.88 Link here | One used in class so programming is easier Supply voltage and output are all within the range needed Lots of documentation Up to 6A output  | Limited on motors that are compatible with this device Limited to only SPI and PWM communication |
| # Option 2. NCV7544MWTXG Price: $4.21 Link here   | Fits requirements of part Can control multiple motors at once  16-bit SPI                                                                   | Limited to only SPI and PWM communication Required supply voltage over 3V                        |
| # Option 3. TLE9201SGAUMA1 Price: $5.38 Link here | High operating temperature range Compatible with most DC motors  Lots of documentation                                                      | Required supply voltage over 3V Only works with one motor  Limited communication channels        |

### Optimal Solution: IFX9201SGAUMA1
For the motor controller the optimal solution is the IFX9201SGAUMA1. This is because it is the controller we will be working with in class and it allows for all the key features needed from this part. Its ability to be powered by a 3V supply is also a huge advantage compared to the other controllers. Overall this option is the best choice.

## Motor

| Solution                                                                  | Pros                                                                                                                                                                                                             | Cons                                                                                                                                                                   |
|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| # Option 1. 1568-ROB-15277-ND SparkFun Electronics Price: $6.88 Link here | Geared motor allowing for more torque 6-24V input range allowing for it to operate within low and high voltage  Lightweight Product                                                                              | Above logic level voltage Very low RPM 200                                                                                                                             |
| # Option 2. 3871 Adafruit Industries LLC. Price: $1.95 Link here          | Runs between 3-3.7V Meaning it will function with on board power Very small form factor allowing for easy placement within device Unique design would allow for the sensors to easily be mounted on the product. | Not much power compared to the other options Low size means that it might ont be able to hold sensor Low power range means if there is a voltage problem it could fail |
| # Option 3. ROB-13258 Price: $5.50 Link here                              | High voltage input range from 3-6V Unique form factor allow for part to be placed in different areas easily High torque                                                                                          | Low RPM 65 High cost compared to other three options  All plastic internals                                                                                            |

### Optimal Solution: 1568-ROB-15277-ND SparkFun Electronics
The best component found for the motor was the 1568-ROB-15277-ND SparkFun Electronics. This high torque motor will allow for the movement aspect of our project to work efficiently. This is a very cost effective motor that has lots of information scattered across the web in case there is any need for assistance. The gear box inside allows for slow and precise movement of objects that have some weight to them. Overall with its ability to be powered by the 9V main supply and high torque for cost and size this motor is the best option. 

## Linear + Switching Regulator

| Solution                                            | Pros                                                                                      | Cons                                                                                   |
|-----------------------------------------------------|-------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| # Option 1. MAX14750CEWA+T Price: $4.63 Link here   | Has the desired output voltage Surface mount configuration  Reasonable cost               | Has excessive features  Very small compared to the other options Untested by our group |
| Option 2. # Option 2. BD933N1WG-CTR $1.34 Link here | Simple output No excessive features Very reasonable price Chisel tip leads  Surface mount | Untested by Team 305 Minimum 4.5V input                                                |
| # Option 3. LM2575S-3.3/NOPB $4.90/each Link here   | Tested by Team 305 previously in class Desired output current Can output 3.3v             | Relatively high cost High demand  Package is different from what Team 305 is used to.  |

### Optimal Solution: LM2575S-3.3/NOPB
The LM2575S-3.3/NOPB is the ideal choice for Team 305 because of its ease of use, high stock at Mouser, and non-excessive features. Compared to the other options, Option 3 does not have features that Team 305 does not plan to use. Additionally - Option 3 has the desired current and voltage output to power the PIC MCU (3.3 V) and the motor chosen above. 

## AC-DC Wall adapter

| Solution                                               | Pros                                                                                                                  | Cons                                             |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| # Option 1. 4336304932 Price: $12.99/each Link here    | Has the output voltage within motors range – 12V+ High value – comes with 2 wall plugs Reasonable cost                | Very high Voltage  2 A output  Cost is high      |
| Option 2. # Option 2. B09TQLNNSR $13.99/each Link here | Simple output No excessive features Multiple tips for different barrel jack styles Low voltage allows for less danger | Untested by Team 305 Max 5 V output Cost is high |
| # Option 3. B09YRGM86T $4.39/each Link here            | Desired output voltage for motors to be functional Can output 9V Works within voltage regulators range.               | Can only output 1A No overload protection        |

### Optimal Solution: B09YRGM86T
The B09YRGM86T is the ideal choice for Team 305 because of its lower cost and ability to power all necessary systems effectively. The other options are either too high or low in current and voltage output making the choice clear. Option 3 is also the most cost effective allowing for the team to spend money elsewhere.  

[click here to return to index](/index)
