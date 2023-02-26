# Microcontroller Selection



| ## 1. Determine your project-specific requirements                              |                                                                               | 3. Look up specifications in the PIC datasheet |                        |                        |
|------------------------------------------------------------------------------|-------------------------------------------------------------------------------|------------------------------------------------|------------------------|------------------------|
| Design Considerations                                                        | Team Project-Specific Requirements  from Problem Definition and Block Diagram | PIC Option 1                                   | PIC Option 2           | PIC Option 3           |
| How many GPIO Pins?                                                          |                                                                               | 60 I/O Pins                                    | 36 I/O Pins            | 85 I/O Pins            |
| Built-in Analog to Digital Converter? How many?                              |                                                                               | 4 Internal 47 external                         | 4 internal 35 external | 4 internal 35 external |
| Built-in Hardware PWM? How many?                                             |                                                                               | 2                                              | 2                      | 1                      |
| Built-in I2C? SPI? How many?                                                 | We need at least 2 serial sensors and 1 serial actuator using I2C or SPI.     | 2                                              | 2                      | 3                      |
| Built-in UART? How many?                                                     | We need at least 1 example of UART, SPI, and I2C.                             | 5                                              | 2                      | 3                      |
| Other Required Built-In Features? (optional)                                 |                                                                               |                                                |                        |                        |
| Additional considerations specific to your project specifications (optional) |                                                                               |                                                |                        |                        |
 3. Look up specifications in the PIC datasheet |                        |                        |
| Design Considerations                                                        | Team Project-Specific Requirements  from Problem Definition and Block Diagram | PIC Option 1                                   | PIC Option 2           | PIC Option 3           |
| How many GPIO Pins?                                                          |                                                                               | 60 I/O Pins                                    | 36 I/O Pins            | 85 I/O Pins            |
| Built-in Analog to Digital Converter? How many?                              |                                                                               | 4 Internal 47 external                         | 4 internal 35 external | 4 internal 35 external |
| Built-in Hardware PWM? How many?                                             |                                                                               | 2                                              | 2                      | 1                      |
| Built-in I2C? SPI? How many?                                                 | We need at least 2 serial sensors and 1 serial actuator using I2C or SPI.     | 2                                              | 2                      | 3                      |
| Built-in UART? How many?                                                     | We need at least 1 example of UART, SPI, and I2C.                             | 5                                              | 2                      | 3                      |
                                                |                        |                        |


## 2. Final Microcontroller Choice: PIC18F67K40
Rationale: Team 305 decided that the PIC18F67K40 IC was the overall best choice for our chosen project. Despite the relatively lower ADC resolution, the amount of pins that the IC has as well as the multitude of packages available make the PIC18F67K40 the right pick for the project. The large amount of pins available in the IC allow for a large degree of freedom and flexibility in where the sensors and other components are located on the PCB. The array of packages available to choose from allow for a perfect selection as to exactly what is needed for the project.

[click here to return to index](/index)
