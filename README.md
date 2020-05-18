# Documentation
[About ThermoMetric Shield](https://github.com/TermoShield/Documentation#about-the-thermo-shield)
[3D shield casing](https://github.com/TermoShield/Documentation#3d-shield-casing)
[Printed circuit board](https://github.com/TermoShield/Documentation#printed-circuit-board)
[Circuit design](https://github.com/TermoShield/Documentation#circuit-design)
[List of components](https://github.com/TermoShield/Documentation#list-of-components)
[Credits](https://github.com/TermoShield/Documentation#credits)

## Thermo-Shield
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1") 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1") 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1") 

### About the Thermo-Shield
The Thermo-Shield for arduino allows a board to acquire environmental data collected by an array of sensors. These sensors consist of thermocouple, IR sensor, digital thermometer, analog temperature sensor and resistance temperature detector.

## Hardware

### 3D shield casing 
We design a 3D visualization of our thermo-shield using the Fusion 360 cloud-based 3D CAD/CAM software which allowed us to better approach real-world problems right away from comfort of our home. Our specialized team produced astonishing model for our arduino shield project. The dimensions of this particular prototype are: ..x..x.. The process of homogenization is achieved through pair of vents that make a circulation and flow of hot air created by Peltier cooling module mainly focused on installed sensors and supported by an inner radiator. The air flows through sophicticated air channel at the bottom of the wall between the vents and the sensors. The air with appropriate temperature is distributed to chamber so that every sensor has equal conditions. All of the componets are packed to lightweight materials to secure transferability as well as maneuverability. This was the demanded property. Several additional changes were made to protect both the PCB and the componets of the external energy sources. The goal that we have been searching for was acceptable balance between the price and those two factors. The last but not least was the issue of maintanance that expected the whole product to be easy to repair if necessary. Our skilled specialist took lead of this approach and came up with the following design. 

![alt text](https://i.imgur.com/hIZOfO8.png "3D model") 

### Printed circuit board
![alt text](https://i.imgur.com/hhH9iUO.png "PCB") 

### Circuit design
The circuit schematics has been designed in the DIPTrace CAD software. You may download the circuit schematics for ThermoMetric shield the  from link below.
```
circuit schematics https://github.com/TermoShield/Elektro/blob/master/ThermoShield_v2.dch
```
The power circuitry is powered by a metal-oxide semiconductor field-effect transistor (MOSFET) Q1 connected to the PWM capable D3 pin of the Arduino. A series resistor R5 protects the MCU U1 in transients, while a resistor R6 parallel to ground ensures that floating electrical states do not cause the heater to turn off accidentally.

Normal temperatures used to melt plastics in 3D printing are over 200°C and may reach as high as 320°C for polycarbonate filaments. To make the experiment safer for general classroom use, the maximal temperature of the heating block is limited at ~80°C by an adjustable linear voltage regulator U2, which takes the external 12V input from the Vin pin of the MCU and reduces it to a voltage configured by resistors R3 and R4 supplying its adjustable input.

Temperature feedback is based on a negative temperature coefficient (NTC) thermistor R1 connected to the A0 analog input pin of the MCU in a voltage divider circuit paired with a resistor R2.

The exact component specification and required quantities are given next. Note that only components with through-hole technology (THT) mounting are utilized in order to make assembly and servicing easy even if you are inexperienced with electronics.

![alt text](https://i.imgur.com/sbr4ik7.jpg "Electric schematic layout") 


### List of components

| Component     | Price         | Quantity |
| ------------- |:-------------:| -----:|     
| Peltierov článok TES1-127021* | 11.93€ | 1x |   
| Chladič V4330K* | 1.77€      |   3x |    
| Ventilátor MF35101V1-10000-A99* | 4.69€      |    2x |   
| Teplovodivá pasta SIL.SE307* | 2.72€ | 1x |
| Vykurovacie teleso TF70 12V/10W* | 14.99€ | 1x |
| Napájací adaptér sieťový 12V 2500mA* | 9.80€ | 1x |
| Tranzistor riadený poľom BTS117* | 2.21€ | 3x |
| Pojistka trubičková GL1.2,5A/E* | 0.11€ | 1x |
| MLX90614 ESF infra sensor* | 12.71€ | 1x |
| DS18B20 - číslicový teplomer* | 1.61€ | 1x |
| MCP9808-E/MS* | 1.09€ | 1x |
| TMP36GT9Z - snímač teploty* | 1.38€ | 1x |
| Rezistor ROYAL OHM 0805S8J0103T5E* | 0.0014€ | 7x |
| Rezistor ERA8AEB1650V* | 0.12€ | 3x |
| PCB* | 0.10€ | 1x |
| Capacitor 0.1 uF* | 0.02€ | 2x |
| Capacitor 1 uF* | 0.05€ | 1x |
| PJ-002A Jack* | 0.22€ | 1x |
| Thermocouple MAX6675* | 7.80€ | 1x |
| Dióda ES1D 1A* | 0.11€ | 5x |
| Thermistor NTC B57164K0101* | 0.51€ | 1x |
| Držiak na poistku Littelfuse 65600001029* | 1€ | 1x |
| **Total amount** | **88.30€** | 

## Software
### Installation:
```
git clone https://github.com/TermoShield
```
or download the zip.

## Credits
### List personnel
+ Martin Žlnay
+ Marek Horník 
+ Michal Mike Masaryk 
+ Marek Sulír 
+ Mišo Vico 
+ Marek Noga 
+ Peter Fábry
