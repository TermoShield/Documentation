# Documentation

### Contents
[About ThermoMetric Shield](#about-the-thermo-shield)<br/>
[3D shield casing](#3d-shield-casing)<br/>
[Printed circuit board](#printed-circuit-board)<br/>
[Circuit design](#circuit-design)<br/>
[List of components](#list-of-components)<br/>
[Credits](#credits)<br/>

## ThermoMetric Shield
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1") 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1") 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1") 

### About the ThermoMetric Shield
The ThermoMetris Shield belongs to the family of control engineering education devices for Arduino that form a part of the [AutomationShield](https://github.com/gergelytakacs/AutomationShield/wiki) project. The Thermo-Shield for arduino allows a board to acquire environmental data collected by an array of sensors. These sensors consist of thermocouple, IR sensor, digital thermometer, analog temperature sensor and resistance temperature detector. This shield relies on the MAX6675 thermocouple digital interface and allows a board to acquire temperatures from a thermocouple of type K and a DS18B20 digital one wire sensor.

## Hardware

### 3D shield casing 
We design a 3D visualization of our thermo-shield using the [Fusion 360](https://www.autodesk.com/products/fusion-360/overview) cloud-based 3D CAD/CAM software. It si a Freeware software. Our specialized team produced model for our arduino shield project. The dimensions of this particular prototype are: ..x..x.. The process of homogenization is achieved through pair of vents that make a circulation and flow of hot air created by Peltier cooling module mainly focused on installed sensors and supported by an inner radiator. The air flows through sophicticated air channel at the bottom of the wall between the vents and the sensors. The air with appropriate temperature is distributed to chamber so that every sensor has equal conditions. All of the componets are packed to lightweight materials to secure transferability as well as maneuverability. This was the demanded property. Several additional changes were made to protect both the PCB and the componets of the external energy sources. The last but not least was the issue of maintanance that expected the whole product to be easy to repair if necessary. Our specialist took lead of this approach and came up with the following design. Can be downloaded [here](https://github.com/gergelytakacs/AutomationShield/wiki/file/Thermo/Complet-assemblery-v11.rar)

![alt text](https://github.com/gergelytakacs/AutomationShield/wiki/fig/3D_model_ThermoMetricShield.png "3D model") 

### Printed circuit board
The printed circuit board has been designed in the Freeware version of the [DIPTrace](https://diptrace.com/) CAD software. The PCB is two-layer and fits within the customary 100x100mm limit of most board manufacturers. The DIPTrace PCB layout and circuit schematics can be downloaded [here](https://github.com/gergelytakacs/AutomationShield/wiki/file/Thermo/ThermoShield_PCB2.1.rar).

![alt text](https://github.com/gergelytakacs/AutomationShield/wiki/fig/ThemoShield_pcb2.3.png =100x20 "PCB")
![alt text](https://github.com/gergelytakacs/AutomationShield/wiki/fig/pcb_bottom_thermoshield.png =100x20 "PCB")

### Circuit design
The circuit schematics has been designed in the DIPTrace CAD software. You may download the circuit schematics for ThermoMetric shield the  from link below. Circuit schematics to download [here](https://github.com/gergelytakacs/AutomationShield/wiki/file/Thermo/ThermoShield_Circuit_v2.rar).

The power circuitry is powered by a metal-oxide semiconductor field-effect transistor (MOSFET) BTS117 connected to the PWM capable D3 pin of the Arduino. A parrarel resistor R5 protects the Peltier plate - thermoelectric sink (TES1-XXXXXX) in transients, while a resistor R6 parallel to ground ensures that floating electrical states do not cause the heater to turn off accidentally.

Normal temperatures used to melt plastics in 3D printing are over 200°C and may reach as high as 245°C for polycarbonate filaments. To make the experiment safer for general classroom use, the maximal temperature of the heating block TF70 is limited by an adjustable voltage regulator, which takes the external 12V input through PJ002A jack.

Temperature feedback is based on a negative temperature coefficient (NTC) thermistor BT2 connected to the A0 analog input pin of the MCU in a voltage divider circuit paired with a resistor R1.


![alt text](https://github.com/gergelytakacs/AutomationShield/wiki/fig/ThermoShield_circuit_v2.jpg "Electric schematic layout") 


### List of components

| Component     | Price         | Quantity | 
| ------------- |:-------------:| :-----:|    
| [Thermoelectric cooling TES1-127021](https://www.conrad.sk/peltierov-clanok-tru-components-tes1-127021-15-4-v-dc-2-1-a-18-1-w.k1569028) | 11.93€ | 1x | 
| [Heatsinks V4330K](https://www.gme.sk/v4330k) | 1.77€      |   3x |   
| [Fan MF35101V1-10000-A99](https://www.gme.sk/mf35101v1-10000-a99) | 4.69€      |    2x |   
| [Heat conducting paste SIL.SE307](https://www.gme.sk/teplovodiva-pasta-sil-se307-white-5g) | 2.72€ | 1x |
| [Heater TF70 12V/20W](https://www.hudiny.sk/12v-20w-mini-ploche-vyhrevne-teleso-26x38mm.html) | 14.99€ | 1x |
| [Power supply 12V 2500mA](https://www.gme.sk/napajeci-adapter-sitovy-12v-2500ma-5-5-2-1mm-b-vigan) | 9.80€ | 1x |
| [HITFET BTS117](https://www.gme.sk/unipolarni-tranzistor-bts117-to220) | 2.21€ | 3x |
| [Tube fuse GL1.2,5A/E](https://www.gme.sk/pojistka-trubickova-gl1-2-5a-e?fbclid=IwAR26pUEECM1JgIv6eXmfsC3xKBfPMm5lMTgnZXRuTRgRJyvqPDXqCdsb1Dk) | 0.11€ | 1x |
| [DS18B20 - Digital Thermometer](https://www.gme.sk/ds18b20) | 1.61€ | 1x |
| [Digital Temperature Sensor MCP9808-E/MS](https://www.distrelec.sk/sk/snimac-teploty-microchip-mcp9808-ms/p/17336047) | 1.09€ | 1x |
| [TMP36GT9Z - Temperature Sensor (Analog)](https://www.gme.sk/tmp36gt9z) | 1.38€ | 1x |
| [Resistor ROYAL OHM 0805S8J0103T5E](https://www.tme.eu/sk/details/smd0805-10k/rezistory-smd-0805/royal-ohm/0805s8j0103t5e/) | 0.0014€ | 7x |
| [Resistor ERA8AEB1650V](https://cz.farnell.com/panasonic/era8aeb1650v/res-165r-0-1-0-25w-1206-thin-film/dp/2094951) | 0.12€ | 3x |
| PCB | 0.10€ | 1x |
| [Capacitor 0.1 uF](https://www.sparkfun.com/products/8375) | 0.02€ | 2x |
| [Capacitor 1 uF](https://sk.farnell.com/panasonic/ecqv1h105jl/capacitor-film-50v-1uf/dp/1744833) | 0.05€ | 1x |
| [PJ-002A Jack](https://www.mouser.sk/ProductDetail/CUI-Devices/PJ-002A?qs=WyjlAZoYn51CKfAix9Mngw==) | 0.22€ | 1x |
| [Thermocouple MAX6675](https://www.ebay.com/itm/MAX6675-Module-K-Type-Thermocouple-Temperature-Sensor-for-Arduino-AL-/400798924042) | 7.80€ | 1x |
| [Diode ES1D 1A](https://www.gme.sk/dioda-es1d) | 0.11€ | 5x |
| [Thermistor NTC B57164K0101](https://www.gme.sk/termistor-ntc-b57164k0101) | 0.51€ | 1x |
| [Fuse Holder Littelfuse 65600001029](https://www.mouser.sk/ProductDetail/Littelfuse/65600001029?qs=Vv6sT79n3zSxfay18w9fWw==) | 1€ | 1x |
| **Total amount** | **88.30€** | 

## Software
### Installation:
```
git clone https://github.com/TermoShield
```
or download the zip.

## Credits
### List personnel
**Hardware design:** Marek Horník, Michal Masaryk, Michal Vico, Marek Noga, Martin Žlnay

**3D model design:** Peter Fábry, Marek Sulír 

**Wiki:** Daniel Fazekas, Martin Žlnay
 

 


