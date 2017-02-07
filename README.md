# ProtoCentral Kalam v3 IOT platform

ProtoCentral Kalam v3 is our newest IOT platform based on the ESP8266 Wi-Fi SoC. It's easy-to-use, low cost and easily scalable. 

IoT is now made easy with quick plug-and-play functionality in both hardware and software. Based on the popular ESP8266 Wi-Fi SoC from Espressif, this board contains everything required, right out of the box.

![Kalam v3](/docs/images/protocentral-kalam-v3.jpg)

Features
--------
* ESP8266EX WiFi System-on-Chip (SoC) with ARM Cortex M3 microcontroller
* On-board 2.4 GHz PCB antenna
* FTDI-based USB-UART interface with microUSB connector
* Fully compatible with the Arduino IDE
* Single Li-Ion battery powered
* On-board battery charger
* 31-pin Hirose DF-9 connector on the back for expansion

Repository Contents
-------------------
* **/hardware** - All Eagle design files (.brd, .sch)
* **/libraries** - Arduino libraries and example code
* **/docs** - Additional Documentation

Board Overview
--------------
![Kalam labelled](/docs/images/kalam-labelled.jpg)

Getting Started with Kalam
--------------------------
Connect the GPIO expaner cap to the Kalam V3 by stacking it on top.Now that the setup is complete,the setup needs to be powered up.Attach a Li-poly battery to the Kalam v2 Iot board.Control the power using the on/off switch

How to setup Arduino support for Kalam (using Sparkfun thing Dev)
---------------------------------------------------
Kalam is powered by the Sparkfun's board support file.The first thing you will need to do is to download the latest release of the Arduino IDE. You will need to be using version 1.6.4 or higher. 
After you have downloaded and installed v1.6.4, you will need to start the IDE and navigate to the Preferences menu.
Sparkfun's  JSON url for ESP8266 board is - https://raw.githubusercontent.com/sparkfun/Arduino_Boards/master/IDE_Board_Manager/package_sparkfun_index.json

![Json](/docs/images/json.jpg)

* Click Ok to close and save the preferences
* Then click Tools > Board > Board Manager
* You should find Sparkfun ESP8266 boards listed in the Board Manager window.

 ![board_manager](/docs/images/boardmanager.png)
 
*	Press the “Install” button on the chosen ESP8266 category.The download process will begin
* Reboot Arduino and look under Tools > Boards and you should see the addition of the Sparkfun boards in your board list.
![board](/docs/images/board.png)

Getting Started with ThingSpeak
-------------------------------
The Internet of Things (IoT) provides access to a broad range of embedded devices and web services. ThingSpeak is an IoT platform that enables you to collect, store, analyze, visualize, and act on data from sensors or actuators.The primary element of ThingSpeak activity is the channel, which contains data fields, location fields, and a status field. After you create a ThingSpeak channel, you can write data to the channel, process and view the data  and react to the data.

Setup ThingSpeak
----------------
ThingSpeak requires a user account and a channel. A channel is where you send data and where ThingSpeak stores data. Each channel has up to 8 data fields, location fields, and a status field. You can send data every 15 seconds to ThingSpeak.

* Sign up for new User Account – https://thingspeak.com/users/sign_up

![signup](/docs/images/signup.jpg)

* Create a new Channel by selecting Channels, My Channels, and then New Channel

![newchannel](/docs/images/creating channel.JPG)

You can change the name to fit your need and you can add a description corresponding to the channel. You can add any other useful description into the metadata field. In the same page, you should see the fields for Latitude, Longitude and Elevation. Also, you can make the channel as "Private" or "Public".

![channel](/docs/images/channel.jpg)

Once you have edited the fields, click on ‘Save Channel’ button.
License Information
-------------------
This product is open source!

Please use, reuse, and modify these files as you see fit. Please maintain attribution to Protocentral and release anything derivative under the same license.
