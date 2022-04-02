#Project Proposal

##Abstract
This air quality monitoring project for [IAL622] is designed around the Arduino MKR WiFi 1010 board. This board uses a [SAMD21 microcontroller], which can be found in other boards, including the Arduino [MKR family], Arduino [Zero], and Adafruit [Feather M0 family].

The MKR WiFi 1010 board provides many advantages over other Arduino-based boards. The MKR WiFi 1010 supports WiFi and Bluetooth Low Energy for wireless connectivity and has a 5-pin JST ESLOV connector to allow rapid-prototyping with sensors that use any of the [STEMMA] / [STEMMA QT] / [Qwiic] / [Gravity] / [Grove] connectors. 

The MKR 485 Shield is one of the few ways to connect RS485 based devices to an Arduino. The low-cost DFRobot Wind Direction Transmitter uses RS485 as its interface. A BME688-based sensor captures temperature, humidity, barometric pressure , and the overall level of volatile organic compounds (VOC). A PMSA003I-based sensor uses laser scattering to measure the concentrations of particulate matter in the air.  The I2S MEMS microphone sensor captures digital audio via the I2S bus. The BME688 and PMSA003I sensors from Adafruit uses STEMMA QT connectors, while the I2S MEMS microphone will be connected via a breadboard or soldered.

The MKR WiFi1010 is “cloud compatible board” and supported by Arduino IoT Cloud, an easy-to-use platform for collecting, monitoring, and visualizing the data. Temperature, humidity, pressure, VOC level, PM1.0, PM2.5, PM10.0, wind direction will be collected. Digital sound will be captured and spectrum-analyzed in an attempt to detect varying levels and frequency of vehicle and train traffic.

The motivation behind the project is concerns about the air quality at our apartment. On many mornings the air smells like the apartment community has been repainted, but there has not been any painting. My partner is sensitive to odors and air quality and experiences headaches and asthma symptoms when the air quality is perceived as poor. This project attempts to find a correlation between perceived air quality and measurable factors affecting air quality. It is hypothesized that location is a contributing factor. Many VOCs and particulate matter are denser than air and our apartment on River Bottom Road is literally in a river bottom, which could encourage air pollutants to collect here. Both NC-55, a four-lane divided highway, and a CSX railroad line, which carries both CXS freight and Amtrak passenger trains, pass within 250 meters of our apartment.

Practical applications for this project and the data collected may include predictive models of local air quality, allowing one to make informed decisions about better times to open windows or engage in outdoor activities. The data collected could be used to inform policy decisions relating to regional air quality issues. 

##Components and supplies
###Devices
* [Arduino MKR WiFi 1010]
* [Arduino MKR 485 Shield]
###Sensors
* [DFROBOT SEN0482] RS485 Wind Direction Transmitter
* [Adafruit BME688] - Temperature, Humidity, Pressure and Gas Sensor
* [Adafruit PMSA003I] - Air Quality Breakout
* [Adafruit I2S MEMS] - Microphone Breakout
###Parts
* [STEMMA QT / Qwiic JST SH 4-pin Cable]
* [5V 2.5A Switching Power Supply] with 20AWG MicroUSB Cable
* [Adafruit Parts Pal]
###Dashboard
* [Arduino IoT Cloud]
