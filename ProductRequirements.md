---
title: Product Requirements 
---

# 3.0 Product Requirements

## 3.1 Objective

Team 305’s objective is to design a reliable weather monitoring system that is capable of monitoring its surroundings, recording and transmitting data, and resisting environmental wear. The primary goals of Team 305 are to meet the requirements of EGR 314, while also working towards improving our skill sets and learning new skills. Although selling the final product would be great, it is not the primary focus of the team. Team 305 has established that the finished product is non-competitive and is purely an academic exercise for the purposes of EGR 314. 

The weather monitoring system developed by Team 305 utilizes two serial sensors and a motor controlled actuator that communicate through I2C and SPI. Most of the original goal were met, which included: creating a fully operational product that ensures all sensors and components function as intended, giving the product a professional appearance, meeting all EGR 314 goals and requirements, enhancing each team member’s skills and encouraging skill development, and designing a cost effective and uncomplicated product.

In summary, Team 305’s weather monitoring system utilizes an ESP32 microcontroller to handle data from the sensors. It sends the data to an online repository and can update values live. All subsystems function and have been verified individually. The original product requirements still apply - though some have been omitted that were no longer relevant to the product design. 

## 3.2 Stakeholders

Due to the non-competitive nature of this group stakeholders are limited to ASU affiliates, including involved students, professors, and potential private interests. 

**Target Group:** Commercial and hobbyist growers.

**Target Purchaser/User:** Residential and commercial greenhouse or grow tent users.

**Regulatory instances:** Meet EGR 314 Spring 2023 requirements and ASU Code of Conduct for Engineers.

## 3.3 Use Cases

**User #1: Rick**

Rick is a 30 year old homeowner who lives in Phoenix, Arizona. Since the temperatures in Arizona are harsh he decided to build a greenhouse in his backyard. He uses Team 305’s weather control module to regulate his greenhouse’s temperature and light levels so that he can achieve the best possible plant development. On his smartphone, Rick launches the weather app of Team 305 and checks the most recent data on the conditions within the greenhouse. The temperature and light parameters can then be adjusted based on his data monitoring to the values he desires.

**User #2:  Samantha**

Samantha is a young adult who is 25 and currently works at “Living Carbon”. This company is located in San Francisco, California. Samantha's position is called plant care associate and she is in charge of research and growth in greenhouses. Her new project is to test out Team 305’s weather control module. She will alter the temperature and light levels to see how well the sensors are performing. With this weather control module she can use the Wi-Fi controlled app that will send live data in the greenhouse conditions. Samantha can monitor the data remotely in this way.

## 3.4 Aspects

The following product aspects encompass the core functionality of the Team 305 weather station project. These aspects have been ranked based on their priority – 5 being the highest priority and 1 being the lowest priority. 

1. **Hardware / Product Design:** The design and hardware of the module weather station should meet these requirements
    1. The product will be simple in design and not time consuming to fix. (5)
    2. The product will have a variety of sensors. (5)
    3. The product will have wheels for a motor actuation. (4)
    4. The product will have a power supply and with batteries. (3)
2. **Software / Functionality:** The product’s software and functionality must be able to meet these standards
    1. The product will connect to and send data over Wi-Fi. (5)
    2. The product will produce reliable and accurate data. (4)
    3. The product’s motors are bidirectional and allow for some manual control. (4)
    4. The products UI/System will be easy to understand, ages < 12 years should understand. (3)
    5. The product will have a long battery life. (3)
3. **Interactivity:** The Users should be able to easily interact with the product by meeting these requirements.
    1. The product will be easy to set up. (5)
    2. The product is easy to use. (5)
    3. Users have easy access to the database where data is sent. (4)
    4. The UI for the product will be easy to understand and is intuitive. (4)
    5. The product will send a warning if one sensor is not reading. (3)
4. **Customization:** Customization of the product will meet these standards in order to be seen as successful. 
    1. The product's sensors will be easily replaced(5)
    2. The product can hang from the ceiling. (4)
5. **Manufacturing:** Product manufacturing must meet these standards. 
    1. The overall product will be built for longevity. (5)
    2. The sensors are robust and do not break easily. (4)
    3. The product will be affordable to construct. (4)
6. **Safety:** The product needs to meet these safety requirements in order to be produced.
    1. The product will not have any exposed direct current that could endanger users. (5)
    2. The product will have fuses or fail-safes in cases of too much power running through parts. (5)
    3. The product will be powered on no higher than 3.3v based on products. (5)
    4. The wires used within the product will be hidden unless directly needed. (4)
    5. The product works without errors.(4)


## 3.5 Open Questions

1. When creating the weather module, how accurate can we make the sensors using the components we have?

Answer: The team took efforts to use the data sheets and code to make it as accurate as they could with the components they had.

2. How will we calibrate the sensors initially?

Answer: The sensors are pre-calibrated by the manufacturer. 

3. Does the Motors motion need to be directly visible?

Answer: Yes the motors need  to be directly visible to prove to guests that it is moving.

4. What are sensors that would not be recommended for use in this case?

Answer: Traditional glass thermometers, soil moisture sensors, pyranometers, and sonic anemometers are a few sensors that the team does not advise using. These are mentioned since each component has unique undesirable characteristics. For instance, weak, cumbersome, hefty, and power hungry.

5. What is the expected life span of the sensors on average?

Answer: When it comes to the lifespan of sensors, several factors may be at play. The sensors may endure for years, provided they are in excellent condition and the atmosphere is at the ideal temperature.

## 3.7 Milestones 

3x4 Design Ideation - 01/20/2023

314 Team Checkpoint 1 - 01/23/2023

3x4 Block Diagram - 01/30/2023

3x4 Component - Selection 02/01/2023

314 Microcontroller Selection - 02/08/2023

3x4 Software Proposal - 02/15/2023

3x4 Hardware Proposal - 02/22/2023

3x4 Team Checkpoint 2 - 02/27/2023

314 Team System Prototype - (recommended) - 03/17/2023

3x4 Hardware Implementation - 03/24/2023

314 Team System Prototype - (final deadline) - 03/17/2023

3x4 Software Implementation - 04/19/2023

3x4 System Verification (final deadline) - 04/24/2023

[click here to return to index](/index)
