# UCA_BluePill
Integrated LoRa PCB with BluePill Board


Version 1.0.0, September, 2019
Author: Fabien Ferrero


This PCB was developed to ease connection between an BluePill, and RFM95 LoRa module, AA battery and a printed antenna.

Nice introduction to BluePill in french can be found on :
https://www.supinfo.com/articles/single/8201-debuter-avec-pilule-bleu-stm32


# PCB UCA_BluePill

<img src="https://github.com/FabienFerrero/UCA_BluePill/blob/master/pictures/top.png">

This PCB has been designed to enable the connection of multiple sensors, few possibilities are listed in this figure :

<img src="https://github.com/FabienFerrero/UCA_BluePill/blob/master/pictures/bottom.png">

# Bill Of Material


* BluePill STM32
https://fr.aliexpress.com/item/32525208361.html?spm=a2g0o.productlist.0.0.1f84d2b3ZWiJAK&algo_pvid=bccebdb6-84b0-45c2-876b-078bdb7fecf1&algo_expid=bccebdb6-84b0-45c2-876b-078bdb7fecf1-7&btsid=5111c833-8677-4ba7-b000-8c66ff8b3dd8&ws_ab_test=searchweb0_0,searchweb201602_4,searchweb201603_53
* RFM95W
https://fr.aliexpress.com/item/RFM95W-RFM95-868MHz-LORA-SX1276-wireless-transceiver-module-20DBM-3KM-Best-quality/32810607598.html?spm=a2g0s.9042311.0.0.bMWhGH

Optional :


* BME280 ( temperature, barometer and humidity sensor)
https://fr.aliexpress.com/item/3In1-BME280-GY-BME280-Digital-Sensor-SPI-I2C-Humidity-Temperature-and-Barometric-Pressure-Sensor-Module-1/32830483099.html?spm=a2g0s.9042311.0.0.2GH3nf


# Wiring

```
 BluePill       LoRa RFM95W 
 STM32           Module
 PB3         <----> RST
 PA6         <----> MISO
 PA7         <----> MOSI
 PB6         <----> CLK
 PB4         <----> SEL (Chip Select)
 PC15        <----> DIO0
 PC14        <----> DIO1
 PC13        <----> DIO2
 3.3V        <----> Vcc

 ```

# Layout

The layout of the PCB is available the gerber section.


# License

All rights reserved. This Gerber, program and the accompanying materials are made available under the terms of the MIT License which accompanies this distribution, and is available at https://opensource.org/licenses/mit-license.php
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Maintained by Fabien Ferrero
