# Ce11: Cellerator
OpenSource Laboratory Robot
<p align="center">
<img src="./images/Ce11.gif" width="200">
</p>

This is the online repository for the OpenSource hardware project Cellerator.

[CellEleven website](http://www.celleleven.com/cellerator)|[Cellerator 3D files](https://cad.onshape.com/documents/5c8c29e275c3d6ad24e851a0/w/f1721dd44bb4fc0688265a60/e/036a6ba0b35b22a34429db9e)

**NOTE*** PUT IMAGE OF CELLERATOR NEXT TO LABASSISTANT 

## Introduction

**Cellerator** _a ce11 product_ is a computer controlled laboratory technician that allows precision handling of biological supplies, with the aid of hand tools, and bench tools.  The protocol is validated via images processed by the computer, and data collected from environmental sensors.   All data saved and graphs are published to the community.
    
## Parts of Cellerator
_To help users identify parts, and to teach anatomy, the parts of Cellerator are named after parts of the body with similar functions._

#### Central Nervous System (CNS)
* Brain ----> Raspberry Pi 5V
* Spinal Cord ----> RJ11 Hub and RJ11 Wire, GPIO Pins

#### Peripheral Nervous System (PNS)
* Cranial Nerves ----> RPi: HDMI out, WiFi, Audio Jack, CSi interface [Camera], DSI Port [Touch Screen],
  * *Eye* 8 megapixel Camera is attached to the CSi Port
  * *Eye Muscle* The Pan and Tilt will be connected to GPIO Pin (GND, 3V3, GPIO15, GPIO16)
* Spinal Nerves ----> IC2 Communication Protocol to Arduino Micro Controller
* Sensory ---->  [UART, or SPI (I2C is for PNS)] Arduino can talk to sensors

#### Muscular system
* Muscle ----> [UART, or SPI (I2C is for PNS)] Arduino can talk to steppers, motors, actuators, and power supply
  * gCODE controlled via USB on an Arduino
* Bone ----> Currently extruded aluminum, working on sheet metal.
* Hand ----> 8 GPIO pogo pin (5v, GROUND, GPIO13, GPIO35, GPIO16, GPIO26, GPIO20, GPIO21)
* Finger ----> Grabber for manipulation of items (5v, GROUND, GPIO32)


#### Vital Organs
* Heart ----> 12V 10A Power Supply
  * Cardio Vascular System ----> Wires, RJ11
  * Precapillary sphincters ----> RJ11 Power Relay (12V, GND, DS, SHCP, STCP) GPIO22-25 Shift Register
* Lungs ----> _Gas Tank, CO2 Tank (what about Bioreactor that produces CO2 [yeast] O2 [Algae])_
  * _pending_ Cilia ----> HEPA negative Air-filter
  * _pending_ Diaphragm ----> Air Pump Relay, Air Vacuum Relay (5V, GRD, GPIO22-25 Shift Register)
* _pending_ Skin ----> designed to keep the workspace sterile
* _pending_ Stomach ----> Hot plate, mixing plate, illumination (RGBw), chemical reagent factory.
* _pending_ 
wait -- {Kidney} Centrifuge (I2C)
wait -- {Loop of Henle} Electrophoresis
wait -- {Bladder} Waste fluid tank
wait -- {Reproductive} Bioreactor, Electro Proration

#### Mouth / Face
* Mouth ----> Load Cartridge, Arduino CNC switch?
* Vocal Cords ----> Output Speaker, Wifi
* Salivary gland ----> Water Pump Relay (5V, GND, GPIO22-25 Shift Register)
* Face ----> Output Display
* _Pending Ear_ ----> Sound Sensor (USB Microphone)
* _Pending Nose_ ----> Air Sensor: MQ-135 MQ135 Air Quality Sensor (5V, GND, TTL switch signal output, AO: analog Signal Output)


## Tools

### Hand Tools
_All hand tools contain a QR Code to validate the correct tool is selected regardless of the location_
* Laser
* Pipette
* Loop
* homogenizer
*

### Bench Tools
* 
