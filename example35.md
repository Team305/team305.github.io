---
title: |
  []{#_cw88o31uri3y .anchor}

  []{#_syw7sfz8egjk .anchor}

  []{#_mob80isx3nkw .anchor}

  []{#_g1ya4ky1rzj0 .anchor}**Component Selection**
---

EGR 314 - ASU Polytechnic - Spring 2023

Professor Kelley & Dr. Aukes - *Instructors*

**Team 305:**

Mark Alvarez -- *Meeting Leader*

Tristan Dunton -- *Assignment Leader*

Aaron Karsten -- *Meeting Recorder*

Kevin Hays -- *Project Monitor*

**2/1/23**

## Temperature Sensor

+-----------------------+-----------------------+-----------------------+
| Solution              | Pros                  | Cons                  |
+=======================+=======================+=======================+
| ![](media             | -   Digital Sensor    | -   No SPI            |
| /image11.png){width=" |                       |     > compatibility   |
| 1.4841546369203849in" | -   Wide supple range |                       |
| height="1             |     > 2.7v\~5.5v      | -   No UART           |
| .4918055555555556in"} |                       |     > compatibility   |
|                       | -   Low Power 200µA   |                       |
| Option 1.             |     > operating       |                       |
|                       |     > current         |                       |
| TC74A4-3.3VCTTR       |                       |                       |
| surface mount temp    | -   Thermistor        |                       |
| sensor                |     > Replacement     |                       |
|                       |                       |                       |
| \$1.09/each           | -   I2C compatible    |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| h                     |                       |                       |
| ere]{.underline}](htt |                       |                       |
| ps://www.digikey.com/ |                       |                       |
| en/products/detail/mi |                       |                       |
| crochip-technology/TC |                       |                       |
| 74A4-3-3VCTTR/443268) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](medi              | -   I2C compatible    | -   No SPI            |
| a/image17.png){width= |                       |     > compatibility   |
| "1.453125546806649in" | -   Wide supple range |                       |
| height="              |     > 2.7v\~5.5v      | -   No UART           |
| 1.453125546806649in"} |                       |     > compatibility   |
|                       | -   Temperature range |                       |
| Option 2.             |     > of -40C to      | -   Excessive         |
|                       |     > +125C           |     > features that   |
| TMP175AID surface     |                       |     > would not be    |
| mount temp sensor     | -   Digital Sensor    |     > utilized        |
|                       |                       |                       |
| \$2.65/each           | -   Small 8-Pin MSOP  |                       |
|                       |     > and 8-Pin SOIC  |                       |
| [[Link                |     > Packages        |                       |
| here]{.underli        |                       |                       |
| ne}](https://www.digi |                       |                       |
| key.com/en/products/d |                       |                       |
| etail/texas-instrumen |                       |                       |
| ts/TMP175AID/1670055) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](media             | -   I2C compatible    | -   No SPI            |
| /image13.png){width=" |                       |     > compatibility   |
| 1.3697922134733158in" | -   Wide supple range |                       |
| height="1             |     > 2.7v\~5.5v      | -   No UART           |
| .3614391951006124in"} |                       |     > compatibility   |
|                       | -   Temperature range |                       |
| Option 3.             |     > of -40C to      |                       |
|                       |     > +125C           |                       |
| TMP75AID surface      |                       |                       |
| mount temp sensor     | -   Digital Sensor    |                       |
|                       |                       |                       |
| \$1.44/each           | -   Small 8-Pin MSOP  |                       |
|                       |     > and 8-Pin SOIC  |                       |
| [[Link                |     > Packages        |                       |
| here]{.underl         |                       |                       |
| ine}](https://www.dig |                       |                       |
| ikey.com/en/products/ |                       |                       |
| detail/texas-instrume |                       |                       |
| nts/TMP75AID/1670067) |                       |                       |
+-----------------------+-----------------------+-----------------------+

[Optimal Solution:]{.underline} TC74A4-3.3VCTTR

When selecting a temperature sensor, Option 1 is best for Team 305. The
reason for that is because it checks off all the necessary requirements
needed for a temperature sensor. It is a digital sensor, I2C compatible,
and it runs off low power. Team 305 must pay attention and use as little
power as we can when choosing a component. Option 1 is also available to
Team 305 as a through hole component, which allows us to test it before
PCB design.

## Light Sensor

+-----------------------+-----------------------+-----------------------+
| Solution              | Pros                  | Cons                  |
+=======================+=======================+=======================+
| ![](medi              | -   Has 1.8V supply   | -   Very small        |
| a/image9.png){width=" |     > voltage         |     > dimensions, \~3 |
| 2.0208333333333335in" |                       |     > mm long         |
| height="2             | -   Can read 380 nm   |                       |
| .0277777777777777in"} |     > to 1000 nm      | -   Bottom solder     |
|                       |     > wavelengths     |     > pads, will need |
| Option 1.             |                       |     > to use solder   |
|                       | -   12C compatible    |     > paste           |
| AS7343 L-DLGM         |                       |                       |
|                       | -   13 channels, one  | -   Relatively        |
| \$11.11/each          |     > for each        |     > expensive for   |
|                       |     > wavelength      |     > one sensor      |
| [[Link                |                       |                       |
| here]{.und            |                       |                       |
| erline}](https://www. |                       |                       |
| digikey.com/en/produc |                       |                       |
| ts/detail/ams-osram/A |                       |                       |
| S7343L-DLGM/16724750) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](media             | -   Lower in cost     | -   Smallest option   |
| /image12.png){width=" |                       |     > compared to the |
| 2.0208333333333335in" | -   Uses I2C          |     > other two       |
| height="2             |     > communication   |     > sensors         |
| .0277777777777777in"} |                       |                       |
|                       | -   Operates with the | -   Has a limited     |
| Option 2.             |     > desired 1.8 V   |     > light spectrum  |
|                       |     > to 3.3V supply  |     > range           |
| ADUX1020BCPZRL7       |     > voltage range   |                       |
|                       |                       | -   Bottom solder     |
| \$7.07/each           |                       |     > leads           |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{.underline}](ht |                       |                       |
| tps://www.digikey.com |                       |                       |
| /en/products/detail/a |                       |                       |
| nalog-devices-inc/ADU |                       |                       |
| X1020BCPZRL7/6133455) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](media             | -   Broad light       | -   Most expensive    |
| /image15.png){width=" |     > spectrum range  |     > option compared |
| 2.0208333333333335in" |     > from 380 nm to  |     > to other two    |
| height="2             |     > 1000 nm         |     > sensors         |
| .0277777777777777in"} |                       |                       |
|                       | -   I2C compatible    | -   Some of the light |
| Option 3.             |                       |     > within it\'s    |
|                       | -   Operates with     |     > sensor range is |
| AS7343-DLGM           |     > desirable       |     > not relevant    |
|                       |     > supply voltage  |     > for             |
| \$12.10/each          |     > 1.7V - 1.98 V   |     > agricultural    |
|                       |                       |     > applications    |
| [[Link                | -   14 channels, one  |                       |
| here]{.un             |     > for each        | -   Small dimensions  |
| derline}](https://www |     > wavelength      |     > with bottom     |
| .digikey.com/en/produ |                       |     > solder leads    |
| cts/detail/ams-osram/ |                       |                       |
| AS7343-DLGM/16285737) |                       | -   Most expensive    |
|                       |                       |     > option of the 3 |
|                       |                       |     > sensor options  |
+-----------------------+-----------------------+-----------------------+

[Optimal Solution:]{.underline} AS7343L-DLGM

Option 1 is the best choice for Team 305 - mainly for broad spectrum
capabilities, supply voltage range, and method of communication (I2C).
The data sheet is very descriptive and provides users with application
notes, detailed diagrams, code examples, detailed pin readout, and lots
of other well documented information that is pertinent to Team 305's
application. While it does have considerably small dimensions, it was
one of the only sensors that fit all the needs of Team 305. Option 3 is
almost the exact same chip - however Option 3 has an additional channel
dedicated to a wavelength that Team 305 is not interested in measuring.
For these reasons Team 305 feels that Option 1 will suffice to meet
project requirements, which has less channels than Option 3.

## Motor Controller 

+-----------------------+-----------------------+-----------------------+
| Solution              | Pros                  | Cons                  |
+=======================+=======================+=======================+
| ![](medi              | -   One used in class | -   Limited on motors |
| a/image8.png){width=" |     > so programming  |     > that are        |
| 2.0208333333333335in" |     > is easier       |     > compatible with |
| height="2             |                       |     > this device     |
| .0277777777777777in"} | -   Supply voltage    |                       |
|                       |     > and output are  | -   Limited to only   |
| Option 1.             |     > all within the  |     > SPI and PWM     |
|                       |     > range needed    |     > communication   |
| [I                    |                       |                       |
| FX9201SGAUMA1]{.mark} | -   Lots of           |                       |
|                       |     > documentation   |                       |
| Price: \$4.88         |                       |                       |
|                       | -   Up to 6A output   |                       |
| [[Link                |                       |                       |
| he                    |                       |                       |
| re]{.underline}](http |                       |                       |
| s://www.digikey.com/e |                       |                       |
| n/products/detail/inf |                       |                       |
| ineon-technologies/IF |                       |                       |
| X9201SGAUMA1/5415542) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](medi              | -   Fits requirements | -   Limited to only   |
| a/image2.png){width=" |     > of part         |     > SPI and PWM     |
| 2.0208333333333335in" |                       |     > communication   |
| height="2             | -   Can control       |                       |
| .0277777777777777in"} |     > multiple motors | -   Required supply   |
|                       |     > at once         |     > voltage over 3V |
| Option 2.             |                       |                       |
|                       | -   16-bit SPI        |                       |
| NCV7544MWTXG          |                       |                       |
|                       |                       |                       |
| Price: \$4.21         |                       |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{                |                       |                       |
| .underline}](https:// |                       |                       |
| www.digikey.com/en/pr |                       |                       |
| oducts/detail/onsemi/ |                       |                       |
| NCV7544MWTXG/9829097) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](medi              | -   High operating    | -   Required supply   |
| a/image8.png){width=" |     > temperature     |     > voltage over 3V |
| 2.0208333333333335in" |     > range           |                       |
| height="2             |                       | -   Only works with   |
| .0277777777777777in"} | -   Compatible with   |     > one motor       |
|                       |     > most DC motors  |                       |
| Option 3.             |                       | -   Limited           |
|                       | -   Lots of           |     > communication   |
| TLE9201SGAUMA1        |     > documentation   |     > channels        |
|                       |                       |                       |
| Price: \$5.38         |                       |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| he                    |                       |                       |
| re]{.underline}](http |                       |                       |
| s://www.digikey.com/e |                       |                       |
| n/products/detail/inf |                       |                       |
| ineon-technologies/TL |                       |                       |
| E9201SGAUMA1/5960696) |                       |                       |
+-----------------------+-----------------------+-----------------------+

[Optimal Solution:]{.underline} [IFX9201SGAUMA1]{.mark}

For the motor controller the optimal solution is the [IFX9201SGAUMA1.
This is because it is the controller we will be working with in class
and it allows for all the key features needed from this part. Its
ability to be powered by a 3V supply is also a huge advantage compared
to the other controllers. Overall this option is the best
choice.]{.mark}

## Motor

+-----------------------+-----------------------+-----------------------+
| Solution              | Pros                  | Cons                  |
+=======================+=======================+=======================+
| ![](media             | -   Geared motor      | -   Above logic level |
| /image16.png){width=" |     > allowing for    |     > voltage         |
| 2.0208333333333335in" |     > more torque     |                       |
| height="2             |                       | -   Very low RPM 200  |
| .0277777777777777in"} | -   6-24V input range |                       |
|                       |     > allowing for it |                       |
| Option 1.             |     > to operate      |                       |
|                       |     > within low and  |                       |
| 1568-ROB-15277-ND     |     > high voltage    |                       |
|                       |                       |                       |
| SparkFun Electronics  | -   Lightweight       |                       |
|                       |     > Product         |                       |
| Price: \$6.88         |                       |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{.underline}     |                       |                       |
| ](https://www.digikey |                       |                       |
| .com/en/products/deta |                       |                       |
| il/sparkfun-electroni |                       |                       |
| cs/ROB-15277/9995750) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](media             | -   Runs between      | -   Not much power    |
| /image14.png){width=" |     > 3-3.7V Meaning  |     > compared to the |
| 2.0208333333333335in" |     > it will         |     > other options   |
| height="2             |     > function with   |                       |
| .0277777777777777in"} |     > on board power  | -   Low size means    |
|                       |                       |     > that it might   |
| Option 2.             | -   Very small form   |     > ont be able to  |
|                       |     > factor allowing |     > hold sensor     |
| 3871 Adafruit         |     > for easy        |                       |
| Industries LLC.       |     > placement       | -   Low power range   |
|                       |     > within device   |     > means if there  |
| Price: \$1.95         |                       |     > is a voltage    |
|                       | -   Unique design     |     > problem it      |
| [[Link                |     > would allow for |     > could fail      |
| here]{.underlin       |     > the sensors to  |                       |
| e}](https://www.digik |     > easily be       |                       |
| ey.com/en/products/de |     > mounted on the  |                       |
| tail/adafruit-industr |     > product.        |                       |
| ies-llc/3871/9603625) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](media             | -   High voltage      | -   Low RPM 65        |
| /image18.png){width=" |     > input range     |                       |
| 2.0208333333333335in" |     > from 3-6V       | -   High cost         |
| height="2             |                       |     > compared to     |
| .0277777777777777in"} | -   Unique form       |     > other three     |
|                       |     > factor allow    |     > options         |
| Option 3.             |     > for part to be  |                       |
|                       |     > placed in       | -   All plastic       |
| ROB-13258             |     > different areas |     > internals       |
|                       |     > easily          |                       |
| Price: \$5.50         |                       |                       |
|                       | -   High torque       |                       |
| [[Link                |                       |                       |
| here]{.underline}     |                       |                       |
| ](https://www.digikey |                       |                       |
| .com/en/products/deta |                       |                       |
| il/sparkfun-electroni |                       |                       |
| cs/ROB-13258/5684381) |                       |                       |
+-----------------------+-----------------------+-----------------------+

[Optimal Solution:]{.underline} 1568-ROB-15277-ND SparkFun Electronics

The best component found for the motor was the 1568-ROB-15277-ND
SparkFun Electronics. This high torque motor will allow for the movement
aspect of our project to work efficiently. This is a very cost effective
motor that has lots of information scattered across the web in case
there is any need for assistance. The gear box inside allows for slow
and precise movement of objects that have some weight to them. Overall
with its ability to be powered by the 9V main supply and high torque for
cost and size this motor is the best option.

## 

## Linear + Switching Regulator

+-----------------------+-----------------------+-----------------------+
| Solution              | Pros                  | Cons                  |
+=======================+=======================+=======================+
| ![](medi              | -   Has the desired   | -   Has excessive     |
| a/image4.png){width=" |     > output voltage  |     > features        |
| 2.0208333333333335in" |                       |                       |
| height="2             | -   Surface mount     | -   Very small        |
| .0277777777777777in"} |     > configuration   |     > compared to the |
|                       |                       |     > other options   |
| Option 1.             | -   Reasonable cost   |                       |
|                       |                       | -   Untested by our   |
| MAX14750CEWA+T        |                       |     > group           |
|                       |                       |                       |
| Price: \$4.63         |                       |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{.underline      |                       |                       |
| }](https://www.digike |                       |                       |
| y.com/en/products/det |                       |                       |
| ail/analog-devices-in |                       |                       |
| c-maxim-integrated/MA |                       |                       |
| X14750CEWA-T/9833428) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| Option 2.             | -   Simple output     | -   Untested by Team  |
|                       |                       |     > 305             |
| ![](media/image6.     | -   No excessive      |                       |
| png){width="1.5625in" |     > features        | -   Minimum 4.5V      |
| height="1.5625in"}    |                       |     > input           |
|                       | -   Very reasonable   |                       |
| [Option 2.]{.mark}    |     > price           |                       |
|                       |                       |                       |
| [                     | -   Chisel tip leads  |                       |
| BD933N1WG-CTR]{.mark} |                       |                       |
|                       | -   Surface mount     |                       |
| \$1.34                |                       |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{.underline}]    |                       |                       |
| (https://www.mouser.c |                       |                       |
| om/ProductDetail/ROHM |                       |                       |
| -Semiconductor/BD933N |                       |                       |
| 1WG-CTR?qs=tlsG%2FOw5 |                       |                       |
| FFiLuuL0kFG8qg%3D%3D) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](med               | -   Tested by Team    | -   Relatively high   |
| ia/image1.png){width= |     > 305 previously  |     > cost            |
| "1.859375546806649in" |     > in class        |                       |
| height="              |                       | -   High demand       |
| 1.859375546806649in"} | -   Desired output    |                       |
|                       |     > current         | -   Package is        |
| Option 3.             |                       |     > different from  |
|                       | -   Can output 3.3v   |     > what Team 305   |
| LM2575S-3.3/NOPB      |                       |     > is used to.     |
|                       |                       |                       |
| \$4.90/each           |                       |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{.underline}]    |                       |                       |
| (https://www.mouser.c |                       |                       |
| om/ProductDetail/Texa |                       |                       |
| s-Instruments/LM2575S |                       |                       |
| -3.3-NOPB?qs=X1J7HmVL |                       |                       |
| 2ZGH5uY2hHZLXw%3D%3D) |                       |                       |
+-----------------------+-----------------------+-----------------------+

[Optimal Solution:]{.underline} LM2575S-3.3/NOPB

The LM2575S-3.3/NOPB is the ideal choice for Team 305 because of its
ease of use, high stock at Mouser, and non-excessive features. Compared
to the other options, Option 3 does not have features that Team 305 does
not plan to use. Additionally - Option 3 has the desired current and
voltage output to power the PIC MCU (3.3 V) and the motor chosen above.

## AC-DC Wall adapter

+-----------------------+-----------------------+-----------------------+
| Solution              | Pros                  | Cons                  |
+=======================+=======================+=======================+
| ![](medi              | -   Has the output    | -   Very high Voltage |
| a/image5.png){width=" |     > voltage within  |                       |
| 2.0208333333333335in" |     > motors range -- | -   2 A output        |
| height="1             |     > 12V+            |                       |
| .7916666666666667in"} |                       | -   Cost is high      |
|                       | -   High value --     |                       |
| Option 1.             |     > comes with 2    |                       |
|                       |     > wall plugs      |                       |
| 4336304932            |                       |                       |
|                       | -   Reasonable cost   |                       |
| Price: \$12.99/each   |                       |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{.underlin       |                       |                       |
| e}](https://www.amazo |                       |                       |
| n.com/100-240V-Transf |                       |                       |
| ormers-Switching-Appl |                       |                       |
| ications-Connectors/d |                       |                       |
| p/B077PW5JC3/ref=sr_1 |                       |                       |
| _1_sspa?crid=1EM4MOLZ |                       |                       |
| NSYZN&keywords=12v+wa |                       |                       |
| ll+adapter&qid=167743 |                       |                       |
| 6269&sprefix=12v+wa%2 |                       |                       |
| Caps%2C208&sr=8-1-spo |                       |                       |
| ns&psc=1&spLa=ZW5jcnl |                       |                       |
| wdGVkUXVhbGlmaWVyPUEx |                       |                       |
| NE9CMVpOWTFVV040JmVuY |                       |                       |
| 3J5cHRlZElkPUEwMzcxMz |                       |                       |
| U4M0k3RzU1MExKTExONyZ |                       |                       |
| lbmNyeXB0ZWRBZElkPUEw |                       |                       |
| OTE1MzgwMkQ5NU9HU1NXV |                       |                       |
| UVRSiZ3aWRnZXROYW1lPX |                       |                       |
| NwX2F0ZiZhY3Rpb249Y2x |                       |                       |
| pY2tSZWRpcmVjdCZkb05v |                       |                       |
| dExvZ0NsaWNrPXRydWU=) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| Option 2.             | -   Simple output     | -   Untested by Team  |
|                       |                       |     > 305             |
| ![](medi              | -   No excessive      |                       |
| a/image3.png){width=" |     > features        | -   Max 5 V output    |
| 2.0208333333333335in" |                       |                       |
| height="1             | -   Multiple tips for | -   Cost is high      |
| .9722222222222223in"} |     > different       |                       |
|                       |     > barrel jack     |                       |
| [Option 2.]{.mark}    |     > styles          |                       |
|                       |                       |                       |
| [B09TQLNNSR]{.mark}   | -   Low voltage       |                       |
|                       |     > allows for less |                       |
| \$13.99/each          |     > danger          |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| here]{.underline}     |                       |                       |
| ](https://www.amazon. |                       |                       |
| com/PERFEIDY-Charger- |                       |                       |
| Regulated-Transformer |                       |                       |
| -Interchangeable/dp/B |                       |                       |
| 09TQLNNSR/ref=sxin_16 |                       |                       |
| _pa_sp_search_themati |                       |                       |
| c_sspa?content-id=amz |                       |                       |
| n1.sym.17640126-9148- |                       |                       |
| 4700-a727-578cd66ffa9 |                       |                       |
| f%3Aamzn1.sym.1764012 |                       |                       |
| 6-9148-4700-a727-578c |                       |                       |
| d66ffa9f&cv_ct_cx=5v+ |                       |                       |
| wall+power+supply&key |                       |                       |
| words=5v+wall+power+s |                       |                       |
| upply&pd_rd_i=B09TQLN |                       |                       |
| NSR&pd_rd_r=ecf642c4- |                       |                       |
| f535-47c4-84b9-9c7e28 |                       |                       |
| 0800c6&pd_rd_w=xLCnV& |                       |                       |
| pd_rd_wg=qhlW5&pf_rd_ |                       |                       |
| p=17640126-9148-4700- |                       |                       |
| a727-578cd66ffa9f&pf_ |                       |                       |
| rd_r=7FF70AZWAMN5N319 |                       |                       |
| MH22&qid=1677436803&s |                       |                       |
| prefix=5V+wa%2Caps%2C |                       |                       |
| 859&sr=1-2-a73d1c8c-2 |                       |                       |
| fd2-4f19-aa41-2df022b |                       |                       |
| cb241-spons&psc=1&spL |                       |                       |
| a=ZW5jcnlwdGVkUXVhbGl |                       |                       |
| maWVyPUFRQzlRSkFJN0lC |                       |                       |
| T0gmZW5jcnlwdGVkSWQ9Q |                       |                       |
| TAzOTY1NDlON1dMRDNSWT |                       |                       |
| dGWEomZW5jcnlwdGVkQWR |                       |                       |
| JZD1BMDUzOTA5MTFBREg1 |                       |                       |
| SVNFNzdPQksmd2lkZ2V0T |                       |                       |
| mFtZT1zcF9zZWFyY2hfdG |                       |                       |
| hlbWF0aWMmYWN0aW9uPWN |                       |                       |
| saWNrUmVkaXJlY3QmZG9O |                       |                       |
| b3RMb2dDbGljaz10cnVl) |                       |                       |
+-----------------------+-----------------------+-----------------------+
| ![](media             | -   Desired output    | -   Can only output   |
| /image10.png){width=" |     > voltage for     |     > 1A              |
| 2.0208333333333335in" |     > motors to be    |                       |
| height="3             |     > functional      | -   No overload       |
| .0694444444444446in"} |                       |     > protection      |
|                       | -   Can output 9V     |                       |
| Option 3.             |                       |                       |
|                       | -   Works within      |                       |
| [B09YRGM86T]{.mark}   |     > voltage         |                       |
|                       |     > regulators      |                       |
| \$4.39/each           |     > range.          |                       |
|                       |                       |                       |
| [[Link                |                       |                       |
| her                   |                       |                       |
| e]{.underline}](https |                       |                       |
| ://www.amazon.com/Acl |                       |                       |
| orol-100V-240V-5-5mmX |                       |                       |
| 2-5mm-Elliptical-Secu |                       |                       |
| rity/dp/B09YRGM86T/re |                       |                       |
| f=sr_1_5?gclid=Cj0KCQ |                       |                       |
| iAorKfBhC0ARIsAHDzslt |                       |                       |
| CRRGZa2Ene-E88G765J7y |                       |                       |
| 5mwNfMPp0PXX9cqmOCVH6 |                       |                       |
| r3tmDEA8TEaAn1sEALw_w |                       |                       |
| cB&hvadid=17353164501 |                       |                       |
| 3&hvdev=c&hvlocphy=90 |                       |                       |
| 30087&hvnetw=g&hvqmt= |                       |                       |
| e&hvrand=365403739857 |                       |                       |
| 4692265&hvtargid=kwd- |                       |                       |
| 10120937855&hydadcr=1 |                       |                       |
| 9108_9439007&keywords |                       |                       |
| =9v+1a+power+supply&q |                       |                       |
| id=1676511133&sr=8-5) |                       |                       |
+-----------------------+-----------------------+-----------------------+

[Optimal Solution:]{.underline} [B09YRGM86T]{.mark}

The [B09YRGM86T]{.mark} is the ideal choice for Team 305 because of its
lower cost and ability to power all necessary systems effectively. The
other options are either too high or low in current and voltage output
making the choice clear. Option 3 is also the most cost effective
allowing for the team to spend money elsewhere.
