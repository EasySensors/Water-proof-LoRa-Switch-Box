# Water-proof-LoRa-Switch-Box

![arduino waterprof LoRa Switch IP64](https://github.com/EasySensors/Water-proof-LoRa-Switch-Box/blob/master/pics/waterprofLoRaSwitchBoxTop.jpg?raw=true)
![arduino waterprof LoRa Switch IP64](https://github.com/EasySensors/Water-proof-LoRa-Switch-Box/blob/master/pics/waterprofLoRaSwitchBoxIP64.jpg?raw=true)
![arduino waterprof LoRa Switch IP64](https://github.com/EasySensors/Water-proof-LoRa-Switch-Box/blob/master/pics/waterprofLoRaSwitchBoxOpen.jpg?raw=true)

### The Water-proof LoRa Switch Box  is a low cost wireless Arduino IDE compatible (the Atmel ATMega328P) microcontroller with HopeRF LoRa RFM95 or RFM69 433/868/915 radio on-board. Best sutable for Home Automation, IOT. Could be used as switch board for radio controlling any DIY project. You may think of it as Arduino Pro Mini plus all the items in the picture below:

![](https://github.com/EasySensors/switchBox/blob/master/pics/replace2.jpg?raw=true)

# Features & Specifications
### IDE Control: 
- Fully compatible with the Arduino IDE
- Enumerates as an Arduino Pro Mini @ 8 MHz
- Compatible with all RFM 69 \ 95 compatible open source libraries available
### Radio Transceivers:  
Two transceiver options are available
- HopeRF RFM95 LoRa® 433/868/915 MHz (long-range version)
- HopeRF RFM69-HCW 433/868/915 MHz (mid-range version)

### Security: 
- On-board Atmel/Microchip ATSHA204A crypto-authentication chip provides secured handshakes
### Antennas: 
Tuned high performance antenna options that are soldered to the main board
- 915 MHz - United States, Canada, Australia
- 868 MHz - Europe
- 433 MHz - Europe
### Interface: 
- Built-in LED 

### Power: 
Utilizes two CR2032 coin cell batteries
- 4\*AA batteries
- Reverse polarity protection
- High-efficiency power converter
- Batteries can last as long as two years with daily use
- Battery voltage sensor (via divider)
- Sleep current consumption 5uA
- Dimensions 160\*70\*40 mm
- Water-proof, IP 64

 If you find the switch box useful, it is possible to buy it here: [link to buy](https://www.crowdsupply.com/easysensors/easyswitchbox)

**Pin out:** 

Arduino Pins|	Description
------------|--------------
A6 | Connected to Battery voltage sensor (via divider)
A3 | Connected to  ATSHA204A
A4 | DIO1
A5 | Magnet 
D3 Interrupt 1 | Occurs when buttons are pressed
D4 | Connected to LED
D8, A1, D7, A0 | Connected to momentary switch buttons in the left buttons Column
D6, A7, D5, A2 |  Connected to momentary switch buttons in the righ buttons Column 
D9 | RFM restt
D10 | CS
D11 | MOSI
D12 | MISO
D13 | SCK
D2 | DIO0

**Arduino IDE Settings**

![Arduino IDE Settings](https://github.com/EasySensors/ButtonSizeNode/blob/master/pics/IDEsettings.jpg?raw=true)

**programming FTDI adapter connection**

![FTDI Power](https://github.com/EasySensors/SwitchNode/blob/master/pics/FTDIvcc3.jpg?raw=true)

3.3V power option should be used.

### the Arduino example sketches

Easy sensors API sketches. Can use both LoRa RFM95 and RFM69 radios
XXXXXXXXXXXXXXXXXXX.ino  - the switchBox Sketch
XXXXXXXXXXXXXXXXXXX.ino - the receiver serial Gateway Sketch

 [MySensors](https://www.mysensors.org/) API. 

How to use it as home automation (IOT) node controller
------------------------------------------------------

Burn the sketch into and the switchBox will became  one of the MySensors home automation network Node. 
To create the network you need controller and at least two Nodes one as a Sensor, relay or switch Node and the other one as “Gateway Serial”. I personally love [Domoticz](https://domoticz.com/) as conroller. Please check this [HowTo](https://github.com/EasySensors/ButtonSizeNode/blob/master/DomoticzInstallMySensors.md) to install Domoticz.

**Done**

The board is created by  [Koresh](https://www.openhardware.io/user/143/projects/Koresh)


