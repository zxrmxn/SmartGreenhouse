# SmartGreenhouse

# Web-based Condition Monitoring and Automatic Control System of Hydroponic Greenhouse 

This is an IOT project which aims to track greenhouse condition, in addition to "Automatic" greenhouse temperature cooling, a project done for my thesis at IPB Vocational School. This Repository includes Arduino codes and explanation about the system.

![App Screenshot](https://i.ibb.co/1dXtbZP/Potret-Akhir-Luar.jpg) ![App Screenshot](https://i.ibb.co/yqFwS1b/Potret-Akhir-Dalam.jpg)

**Features of project:**

• Monitor the temperature and humidity in the greenhouse, and water TDS content which watering the plants.

• Control the temperature using an automatic electric socket that is connected to a fan and a relay.

 **FULL REPORT:** 
 
 https://drive.google.com/file/d/1T8IwW0b8KGxvV9Kx2R3EW_MFb6P2_stK/view


## 1) Embedded Hardware

This project uses a "ESP8266" as a hardware core.

**Following components are used in the project:**

• ESP8266 

• DHT22

• TDS Meter

• Relay

• Jumper Cable


**DHT Series**

![App Screenshot](https://i.ibb.co/RvGz9vK/rangkaian-dht.png)

DHT22 acts as a sensor that collect both temperature and humidity, the collected data then processed by ESP8266, if the temperature exceed a predetermined limit, relay will automatically activate the fan to cool down the temperature.

• DHT22 data pin connects to ESP8266 D4 pin (Blue cable)

• DHT22 ground pin connect to ESP8266 Ground (Red cable)

• DHT22 vcc pin connects to relay vcc pin (Black cable)

**TDS Series**

![App Screenshot](https://i.ibb.co/1LyCXJ9/rangkaian-tds.png)

TDS sensor serves as a water content detector.

• TDS ground pin connects to ESP8266 ground pin (Red cable)

• TDS vcc pin connects to ESP8266 5v pin (Black cable)

• TDS analog pin connects to ESP8266 A0 pin (Blue cable)

## 2) System Architecture

![App Screenshot](https://i.ibb.co/sm5P7Ng/diagram.png)
## 3) Database

These channels contain data the sensors collected.

![App Screenshot](https://i.ibb.co/VQ5mW3Q/thingspeak.png)
## 4) Website

This is the website interface that shows both grapichal and numerical data of sensors.

![App Screenshot](https://i.ibb.co/MkJbWhN/website.jpg)

**Website URL:** https://iot-biotrop.weebly.com/
## Tech Behind

**Microcontroller:** ESP8266

**Database:** ThingSpeak

**Web Service:** Weebly
