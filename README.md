# UCA_BluePill
Integrated LoRa PCB with BluePill Board


Version 1.0.0, September, 2019
Author: Fabien Ferrero


This PCB was developed to ease connection between an BluePill, and RFM95 LoRa module, AA battery and a printed antenna.


# PCB UCA_BluePill

<img src="https://github.com/FabienFerrero/UCA_BluePill/blob/master/pictures/top.png">

This PCB has been designed to enable the connection of multiple sensors, few possibilities are listed in this figure :

<img src="https://github.com/FabienFerrero/UCA_BluePill/blob/master/pictures/bottom.png">

# Bill Of Material


* BluePill STM32
https://fr.aliexpress.com/item/10pcs-ATMEGA328P-Pro-Mini-328-Mini-ATMEGA328-3-3V-16-MHz-for-Arduino-3-3V-16/32784455996.html?spm=a2g0s.13010208.99999999.276.LOMiw9
* RFM95W
https://fr.aliexpress.com/item/RFM95W-RFM95-868MHz-LORA-SX1276-wireless-transceiver-module-20DBM-3KM-Best-quality/32810607598.html?spm=a2g0s.9042311.0.0.bMWhGH

Optional :


* BME280 ( temperature, barometer and humidity sensor)
https://fr.aliexpress.com/item/3In1-BME280-GY-BME280-Digital-Sensor-SPI-I2C-Humidity-Temperature-and-Barometric-Pressure-Sensor-Module-1/32830483099.html?spm=a2g0s.9042311.0.0.2GH3nf


# Wiring

```
 BluePill       LoRa RFM95W 
 STM32           Module
 D8          <----> RST
 MISO  (D12) <----> MISO
 MOSI  (D11) <----> MOSI
 SCK   (D13) <----> CLK
 SS    (D10) <----> SEL (Chip Select)
 D2          <----> DIO0
 D7          <----> DIO1
 D9          <----> DIO2
 3.3V        <----> Vcc

 ```

# Layout

The layout of the PCB is available the gerber section.


# License

All rights reserved. This Gerber, program and the accompanying materials are made available under the terms of the MIT License which accompanies this distribution, and is available at https://opensource.org/licenses/mit-license.php
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Maintained by Fabien Ferrero
