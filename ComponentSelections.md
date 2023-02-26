---
title: [Component Selection](/index)
---
## Temperature Sensor

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Solution</th>
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image11.png" style="width:1.48415in;height:1.49181in" /></p>
<p>Option 1.</p>
<p>TC74A4-3.3VCTTR surface mount temp sensor</p>
<p>$1.09/each</p>
<p><a href="https://www.digikey.com/en/products/detail/microchip-technology/TC74A4-3-3VCTTR/443268"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Digital Sensor</p>
</blockquote></li>
<li><blockquote>
<p>Wide supple range 2.7v~5.5v</p>
</blockquote></li>
<li><blockquote>
<p>Low Power 200µA operating current</p>
</blockquote></li>
<li><blockquote>
<p>Thermistor Replacement</p>
</blockquote></li>
<li><blockquote>
<p>I2C compatible</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>No SPI compatibility</p>
</blockquote></li>
<li><blockquote>
<p>No UART compatibility</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p><img src="./photos/media/image17.png" style="width:1.45313in;height:1.45313in" /></p>
<p>Option 2.</p>
<p>TMP175AID surface mount temp sensor</p>
<p>$2.65/each</p>
<p><a href="https://www.digikey.com/en/products/detail/texas-instruments/TMP175AID/1670055"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>I2C compatible</p>
</blockquote></li>
<li><blockquote>
<p>Wide supple range 2.7v~5.5v</p>
</blockquote></li>
<li><blockquote>
<p>Temperature range of -40C to +125C</p>
</blockquote></li>
<li><blockquote>
<p>Digital Sensor</p>
</blockquote></li>
<li><blockquote>
<p>Small 8-Pin MSOP and 8-Pin SOIC Packages</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>No SPI compatibility</p>
</blockquote></li>
<li><blockquote>
<p>No UART compatibility</p>
</blockquote></li>
<li><blockquote>
<p>Excessive features that would not be utilized</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image13.png" style="width:1.36979in;height:1.36144in" /></p>
<p>Option 3.</p>
<p>TMP75AID surface mount temp sensor</p>
<p>$1.44/each</p>
<p><a href="https://www.digikey.com/en/products/detail/texas-instruments/TMP75AID/1670067"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>I2C compatible</p>
</blockquote></li>
<li><blockquote>
<p>Wide supple range 2.7v~5.5v</p>
</blockquote></li>
<li><blockquote>
<p>Temperature range of -40C to +125C</p>
</blockquote></li>
<li><blockquote>
<p>Digital Sensor</p>
</blockquote></li>
<li><blockquote>
<p>Small 8-Pin MSOP and 8-Pin SOIC Packages</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>No SPI compatibility</p>
</blockquote></li>
<li><blockquote>
<p>No UART compatibility</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<u>Optimal Solution:</u> TC74A4-3.3VCTTR

When selecting a temperature sensor, Option 1 is best for Team 305. The reason for that is because it checks off all the necessary requirements needed for a temperature sensor. It is a digital sensor, I2C compatible, and it runs off low power. Team 305 must pay attention and use as little power as we can when choosing a component. Option 1 is also available to Team 305 as a through hole component, which allows us to test it before PCB design.

## Light Sensor

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Solution</th>
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image9.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 1.</p>
<p>AS7343 L-DLGM</p>
<p>$11.11/each</p>
<p><a href="https://www.digikey.com/en/products/detail/ams-osram/AS7343L-DLGM/16724750"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Has 1.8V supply voltage</p>
</blockquote></li>
<li><blockquote>
<p>Can read 380 nm to 1000 nm wavelengths</p>
</blockquote></li>
<li><blockquote>
<p>12C compatible</p>
</blockquote></li>
<li><blockquote>
<p>13 channels, one for each wavelength</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Very small dimensions, ~3 mm long</p>
</blockquote></li>
<li><blockquote>
<p>Bottom solder pads, will need to use solder paste</p>
</blockquote></li>
<li><blockquote>
<p>Relatively expensive for one sensor</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p><img src="./photos/media/image12.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 2.</p>
<p>ADUX1020BCPZRL7</p>
<p>$7.07/each</p>
<p><a href="https://www.digikey.com/en/products/detail/analog-devices-inc/ADUX1020BCPZRL7/6133455"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Lower in cost</p>
</blockquote></li>
<li><blockquote>
<p>Uses I2C communication</p>
</blockquote></li>
<li><blockquote>
<p>Operates with the desired 1.8 V to 3.3V supply voltage range</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Smallest option compared to the other two sensors</p>
</blockquote></li>
<li><blockquote>
<p>Has a limited light spectrum range</p>
</blockquote></li>
<li><blockquote>
<p>Bottom solder leads</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image15.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 3.</p>
<p>AS7343-DLGM</p>
<p>$12.10/each</p>
<p><a href="https://www.digikey.com/en/products/detail/ams-osram/AS7343-DLGM/16285737"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Broad light spectrum range from 380 nm to 1000 nm</p>
</blockquote></li>
<li><blockquote>
<p>I2C compatible</p>
</blockquote></li>
<li><blockquote>
<p>Operates with desirable supply voltage 1.7V - 1.98 V</p>
</blockquote></li>
<li><blockquote>
<p>14 channels, one for each wavelength</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Most expensive option compared to other two sensors</p>
</blockquote></li>
<li><blockquote>
<p>Some of the light within it's sensor range is not relevant for agricultural applications</p>
</blockquote></li>
<li><blockquote>
<p>Small dimensions with bottom solder leads</p>
</blockquote></li>
<li><blockquote>
<p>Most expensive option of the 3 sensor options</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<u>Optimal Solution:</u> AS7343L-DLGM

Option 1 is the best choice for Team 305 - mainly for broad spectrum capabilities, supply voltage range, and method of communication (I2C). The data sheet is very descriptive and provides users with application notes, detailed diagrams, code examples, detailed pin readout, and lots of other well documented information that is pertinent to Team 305’s application. While it does have considerably small dimensions, it was one of the only sensors that fit all the needs of Team 305. Option 3 is almost the exact same chip - however Option 3 has an additional channel dedicated to a wavelength that Team 305 is not interested in measuring. For these reasons Team 305 feels that Option 1 will suffice to meet project requirements, which has less channels than Option 3.

## Motor Controller 

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Solution</th>
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image8.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 1.</p>
<p><mark>IFX9201SGAUMA1</mark></p>
<p>Price: $4.88</p>
<p><a href="https://www.digikey.com/en/products/detail/infineon-technologies/IFX9201SGAUMA1/5415542"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>One used in class so programming is easier</p>
</blockquote></li>
<li><blockquote>
<p>Supply voltage and output are all within the range needed</p>
</blockquote></li>
<li><blockquote>
<p>Lots of documentation</p>
</blockquote></li>
<li><blockquote>
<p>Up to 6A output</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Limited on motors that are compatible with this device</p>
</blockquote></li>
<li><blockquote>
<p>Limited to only SPI and PWM communication</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p><img src="./photos/media/image2.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 2.</p>
<p>NCV7544MWTXG</p>
<p>Price: $4.21</p>
<p><a href="https://www.digikey.com/en/products/detail/onsemi/NCV7544MWTXG/9829097"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Fits requirements of part</p>
</blockquote></li>
<li><blockquote>
<p>Can control multiple motors at once</p>
</blockquote></li>
<li><blockquote>
<p>16-bit SPI</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Limited to only SPI and PWM communication</p>
</blockquote></li>
<li><blockquote>
<p>Required supply voltage over 3V</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image8.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 3.</p>
<p>TLE9201SGAUMA1</p>
<p>Price: $5.38</p>
<p><a href="https://www.digikey.com/en/products/detail/infineon-technologies/TLE9201SGAUMA1/5960696"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>High operating temperature range</p>
</blockquote></li>
<li><blockquote>
<p>Compatible with most DC motors</p>
</blockquote></li>
<li><blockquote>
<p>Lots of documentation</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Required supply voltage over 3V</p>
</blockquote></li>
<li><blockquote>
<p>Only works with one motor</p>
</blockquote></li>
<li><blockquote>
<p>Limited communication channels</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<u>Optimal Solution:</u> <span class="mark">IFX9201SGAUMA1</span>

For the motor controller the optimal solution is the <span class="mark">IFX9201SGAUMA1. This is because it is the controller we will be working with in class and it allows for all the key features needed from this part. Its ability to be powered by a 3V supply is also a huge advantage compared to the other controllers. Overall this option is the best choice.</span>

## Motor

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Solution</th>
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image16.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 1.</p>
<p>1568-ROB-15277-ND</p>
<p>SparkFun Electronics</p>
<p>Price: $6.88</p>
<p><a href="https://www.digikey.com/en/products/detail/sparkfun-electronics/ROB-15277/9995750"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Geared motor allowing for more torque</p>
</blockquote></li>
<li><blockquote>
<p>6-24V input range allowing for it to operate within low and high voltage</p>
</blockquote></li>
<li><blockquote>
<p>Lightweight Product</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Above logic level voltage</p>
</blockquote></li>
<li><blockquote>
<p>Very low RPM 200</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p><img src="./photos/media/image14.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 2.</p>
<p>3871 Adafruit Industries LLC.</p>
<p>Price: $1.95</p>
<p><a href="https://www.digikey.com/en/products/detail/adafruit-industries-llc/3871/9603625"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Runs between 3-3.7V Meaning it will function with on board power</p>
</blockquote></li>
<li><blockquote>
<p>Very small form factor allowing for easy placement within device</p>
</blockquote></li>
<li><blockquote>
<p>Unique design would allow for the sensors to easily be mounted on the product.</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Not much power compared to the other options</p>
</blockquote></li>
<li><blockquote>
<p>Low size means that it might ont be able to hold sensor</p>
</blockquote></li>
<li><blockquote>
<p>Low power range means if there is a voltage problem it could fail</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image18.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 3.</p>
<p>ROB-13258</p>
<p>Price: $5.50</p>
<p><a href="https://www.digikey.com/en/products/detail/sparkfun-electronics/ROB-13258/5684381"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>High voltage input range from 3-6V</p>
</blockquote></li>
<li><blockquote>
<p>Unique form factor allow for part to be placed in different areas easily</p>
</blockquote></li>
<li><blockquote>
<p>High torque</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Low RPM 65</p>
</blockquote></li>
<li><blockquote>
<p>High cost compared to other three options</p>
</blockquote></li>
<li><blockquote>
<p>All plastic internals</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<u>Optimal Solution:</u> 1568-ROB-15277-ND SparkFun Electronics

The best component found for the motor was the 1568-ROB-15277-ND SparkFun Electronics. This high torque motor will allow for the movement aspect of our project to work efficiently. This is a very cost effective motor that has lots of information scattered across the web in case there is any need for assistance. The gear box inside allows for slow and precise movement of objects that have some weight to them. Overall with its ability to be powered by the 9V main supply and high torque for cost and size this motor is the best option.

## 

## Linear + Switching Regulator

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Solution</th>
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image4.png" style="width:2.02083in;height:2.02778in" /></p>
<p>Option 1.</p>
<p>MAX14750CEWA+T</p>
<p>Price: $4.63</p>
<p><a href="https://www.digikey.com/en/products/detail/analog-devices-inc-maxim-integrated/MAX14750CEWA-T/9833428"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Has the desired output voltage</p>
</blockquote></li>
<li><blockquote>
<p>Surface mount configuration</p>
</blockquote></li>
<li><blockquote>
<p>Reasonable cost</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Has excessive features</p>
</blockquote></li>
<li><blockquote>
<p>Very small compared to the other options</p>
</blockquote></li>
<li><blockquote>
<p>Untested by our group</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Option 2.</p>
<p><img src="./photos/media/image6.png" style="width:1.5625in;height:1.5625in" /></p>
<p><mark>Option 2.</mark></p>
<p><mark>BD933N1WG-CTR</mark></p>
<p>$1.34</p>
<p><a href="https://www.mouser.com/ProductDetail/ROHM-Semiconductor/BD933N1WG-CTR?qs=tlsG%2FOw5FFiLuuL0kFG8qg%3D%3D"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Simple output</p>
</blockquote></li>
<li><blockquote>
<p>No excessive features</p>
</blockquote></li>
<li><blockquote>
<p>Very reasonable price</p>
</blockquote></li>
<li><blockquote>
<p>Chisel tip leads</p>
</blockquote></li>
<li><blockquote>
<p>Surface mount</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Untested by Team 305</p>
</blockquote></li>
<li><blockquote>
<p>Minimum 4.5V input</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image1.png" style="width:1.85938in;height:1.85938in" /></p>
<p>Option 3.</p>
<p>LM2575S-3.3/NOPB</p>
<p>$4.90/each</p>
<p><a href="https://www.mouser.com/ProductDetail/Texas-Instruments/LM2575S-3.3-NOPB?qs=X1J7HmVL2ZGH5uY2hHZLXw%3D%3D"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Tested by Team 305 previously in class</p>
</blockquote></li>
<li><blockquote>
<p>Desired output current</p>
</blockquote></li>
<li><blockquote>
<p>Can output 3.3v</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Relatively high cost</p>
</blockquote></li>
<li><blockquote>
<p>High demand</p>
</blockquote></li>
<li><blockquote>
<p>Package is different from what Team 305 is used to.</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<u>Optimal Solution:</u> LM2575S-3.3/NOPB

The LM2575S-3.3/NOPB is the ideal choice for Team 305 because of its ease of use, high stock at Mouser, and non-excessive features. Compared to the other options, Option 3 does not have features that Team 305 does not plan to use. Additionally - Option 3 has the desired current and voltage output to power the PIC MCU (3.3 V) and the motor chosen above.

## AC-DC Wall adapter

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Solution</th>
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image5.png" style="width:2.02083in;height:1.79167in" /></p>
<p>Option 1.</p>
<p>4336304932</p>
<p>Price: $12.99/each</p>
<p><a href="https://www.amazon.com/100-240V-Transformers-Switching-Applications-Connectors/dp/B077PW5JC3/ref=sr_1_1_sspa?crid=1EM4MOLZNSYZN&amp;keywords=12v+wall+adapter&amp;qid=1677436269&amp;sprefix=12v+wa%2Caps%2C208&amp;sr=8-1-spons&amp;psc=1&amp;spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUExNE9CMVpOWTFVV040JmVuY3J5cHRlZElkPUEwMzcxMzU4M0k3RzU1MExKTExONyZlbmNyeXB0ZWRBZElkPUEwOTE1MzgwMkQ5NU9HU1NXVUVRSiZ3aWRnZXROYW1lPXNwX2F0ZiZhY3Rpb249Y2xpY2tSZWRpcmVjdCZkb05vdExvZ0NsaWNrPXRydWU="><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Has the output voltage within motors range – 12V+</p>
</blockquote></li>
<li><blockquote>
<p>High value – comes with 2 wall plugs</p>
</blockquote></li>
<li><blockquote>
<p>Reasonable cost</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Very high Voltage</p>
</blockquote></li>
<li><blockquote>
<p>2 A output</p>
</blockquote></li>
<li><blockquote>
<p>Cost is high</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Option 2.</p>
<p><img src="./photos/media/image3.png" style="width:2.02083in;height:1.97222in" /></p>
<p><mark>Option 2.</mark></p>
<p><mark>B09TQLNNSR</mark></p>
<p>$13.99/each</p>
<p><a href="https://www.amazon.com/PERFEIDY-Charger-Regulated-Transformer-Interchangeable/dp/B09TQLNNSR/ref=sxin_16_pa_sp_search_thematic_sspa?content-id=amzn1.sym.17640126-9148-4700-a727-578cd66ffa9f%3Aamzn1.sym.17640126-9148-4700-a727-578cd66ffa9f&amp;cv_ct_cx=5v+wall+power+supply&amp;keywords=5v+wall+power+supply&amp;pd_rd_i=B09TQLNNSR&amp;pd_rd_r=ecf642c4-f535-47c4-84b9-9c7e280800c6&amp;pd_rd_w=xLCnV&amp;pd_rd_wg=qhlW5&amp;pf_rd_p=17640126-9148-4700-a727-578cd66ffa9f&amp;pf_rd_r=7FF70AZWAMN5N319MH22&amp;qid=1677436803&amp;sprefix=5V+wa%2Caps%2C859&amp;sr=1-2-a73d1c8c-2fd2-4f19-aa41-2df022bcb241-spons&amp;psc=1&amp;spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFRQzlRSkFJN0lCT0gmZW5jcnlwdGVkSWQ9QTAzOTY1NDlON1dMRDNSWTdGWEomZW5jcnlwdGVkQWRJZD1BMDUzOTA5MTFBREg1SVNFNzdPQksmd2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWMmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Simple output</p>
</blockquote></li>
<li><blockquote>
<p>No excessive features</p>
</blockquote></li>
<li><blockquote>
<p>Multiple tips for different barrel jack styles</p>
</blockquote></li>
<li><blockquote>
<p>Low voltage allows for less danger</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Untested by Team 305</p>
</blockquote></li>
<li><blockquote>
<p>Max 5 V output</p>
</blockquote></li>
<li><blockquote>
<p>Cost is high</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p><img src="./photos/media/image10.png" style="width:2.02083in;height:3.06944in" /></p>
<p>Option 3.</p>
<p><mark>B09YRGM86T</mark></p>
<p>$4.39/each</p>
<p><a href="https://www.amazon.com/Aclorol-100V-240V-5-5mmX2-5mm-Elliptical-Security/dp/B09YRGM86T/ref=sr_1_5?gclid=Cj0KCQiAorKfBhC0ARIsAHDzsltCRRGZa2Ene-E88G765J7y5mwNfMPp0PXX9cqmOCVH6r3tmDEA8TEaAn1sEALw_wcB&amp;hvadid=173531645013&amp;hvdev=c&amp;hvlocphy=9030087&amp;hvnetw=g&amp;hvqmt=e&amp;hvrand=3654037398574692265&amp;hvtargid=kwd-10120937855&amp;hydadcr=19108_9439007&amp;keywords=9v+1a+power+supply&amp;qid=1676511133&amp;sr=8-5"><u>Link here</u></a></p></th>
<th><ul>
<li><blockquote>
<p>Desired output voltage for motors to be functional</p>
</blockquote></li>
<li><blockquote>
<p>Can output 9V</p>
</blockquote></li>
<li><blockquote>
<p>Works within voltage regulators range.</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Can only output 1A</p>
</blockquote></li>
<li><blockquote>
<p>No overload protection</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<u>Optimal Solution:</u> <span class="mark">B09YRGM86T</span>

The <span class="mark">B09YRGM86T</span> is the ideal choice for Team 305 because of its lower cost and ability to power all necessary systems effectively. The other options are either too high or low in current and voltage output making the choice clear. Option 3 is also the most cost effective allowing for the team to spend money elsewhere.
