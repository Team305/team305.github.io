---
title: Software Proposal
---

# 10.0 Software Proposal 
## 10.1 Software UML Diagram

![Figure 1: Software Proposal Diagram](/photos/SoftwareProposal.jpg "Figure 10a: Software Proposal UML Diagram.")

## 10.2 Software UML Diagram Explanation
Team 305's software proposal is seperated into a myriad of code blocks. The "Main Loop" block is where the climate monitoring system begins on startup. After initializing the internal systems and variables and enabling interrupts, the system does a quick check to see if the subsystems can communicate correctly. If the sensors or motor cannot, the program sends an error code over Wi-fi with appropriate timestamps detailing what subsystem has caused an error and subsequently shuts down. Otherwise, the program continues to the "Environmental Reading" stage. The motor runs, moving the rail and positioning the sensors to take their readings. After taking the initial readings, the motor extends the rail the opposite direction, and the sensors read their environmental data again. The rail is then returned to the initial position. 

After taking the data readings, the program sends said readings to the website over Wi-fi. If for whatever reason the transmit fails, the system illuminates a failed transmit LED to warn the user. Otherwise, it enables a successful transmit LED. In either case, the system then enters a low-power sleep mode for 1 hour before running from the "System Check" block again.

This software proposal has a straightforward, simple design plan that allows for ease of programming and simple debugging. The software proposal also allows for clear data transmission with the use of timestamps, as well as simple and easy to understand user feedback in case something goes wrong.

[click here to return to index](/index)
