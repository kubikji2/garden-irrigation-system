# Garden Irrigation System
All information and codes gathered regarding garden irrigation system goes here.


## Roadmap
Steps and decision required:

### 1. Do research about irrigation systems avialable and choose one

Most of the sources recommends using drip irridation system over watering by hand or using overhead irrigation or sprinklers.
Drip irridation usage saves water, eventhough precise number varies from 75-85% [[1]](https://www.youtube.com/watch?v=NOpvLFwjS1g) to 30-60% [[2]](https://www.dripworks.com/media/wysiwyg/drip-planning-guide.pdf), delivers water near to the plant roots, minimize evaporation and runoffs [[3]](https://www.cdc.gov/healthywater/other/agricultural/types.html), prevents fungal diseas and decrease chance of overwatering as the water is delivered continously overtime[[4]](https://www.youtube.com/watch?v=P86oiKTzuAo).
Additionaly, using drip irridation system can use both presurized [[5]](https://www.youtube.com/watch?v=Bo2GFneYrfM) and non-presurized water source [[6]](https://www.youtube.com/watch?v=WF5TeIQyiHY).
In case of presurized system, it is recommended to use loops without any deadends[[5]](https://www.youtube.com/watch?v=Bo2GFneYrfM).
On the other hand, deadends possible for non-presurized variants as seen in [[6]](https://www.youtube.com/watch?v=WF5TeIQyiHY).
Pressurized version has been controlled using arduino board and selenoid valve by Practical Engineering in [[7]](https://www.youtube.com/watch?v=O_Q1WKCtWiA).

**Sources**:  
[[1]](https://www.youtube.com/watch?v=NOpvLFwjS1g) (Video) How to Build a PVC Drip Irrigation System by _Utah State University Extension_  
[[2]](https://www.dripworks.com/media/wysiwyg/drip-planning-guide.pdf) (Brochoure) Drip planning guide by _Drip Works_  
[[3]](https://www.cdc.gov/healthywater/other/agricultural/types.html) (Site) Types of Agricultural Water Use by _Centers for Disease Control and Prevention_  
[[4]](https://www.youtube.com/watch?v=P86oiKTzuAo) (Video) How to Build a Raised Garden Bed with Drip Irrigation - Inexpensive & Easy by _OrganicBackyardGardening_  
[[5]](https://www.youtube.com/watch?v=Bo2GFneYrfM) (Video) Easy DIY home drip irrigation system by _Adam Woodhams_  
[[6]](https://www.youtube.com/watch?v=WF5TeIQyiHY) (Video) Jesse Explains Gravity Fed Drip Irrigation by _BlueBarrel Rainwater Catchment Systems_   
[[7]](https://www.youtube.com/watch?v=O_Q1WKCtWiA) (Video) Arduino Garden Controller - Automatic Watering and Data Logging by _Practical Engineering_

### 2. Do research about valve types and its usage

Normally closed solenoid two-way valve seems to be way to go for first iteration as it remains closed until given current is applied.
For advanced node-based approach three-way normally closed solenoid valve is preffered.
Controlling a solenoid valve using arduino is described in [[14]](http://www.martyncurrey.com/controlling-a-solenoid-valve-from-an-arduino-updated/).

**Sources**:  
[[11]](https://www.linkedin.com/pulse/different-valve-types-applications-suitability-brian-g-thompson--1) Different Valve Types, Applications & Suitability by _Brian 🇦🇺 Thompson Valve Sage_  
[[12]](https://en.wikipedia.org/wiki/Solenoid_valve) Selenoid Valve by _Wikipedia_  
[[13]](https://www.doityourself.com/stry/5-different-types-of-solenoid-valves-explained) 5 Different Types of Solenoid Valves Explained by _Fiye Ward_  
[[14]](http://www.martyncurrey.com/controlling-a-solenoid-valve-from-an-arduino-updated/) Controlling a Solenoid Valve from an Arduino. Updated by _Martyn Currey_
 

### 3. Do research about Arduino UNO and Arduiono NANO 

Recent version of Arduiono UNO uses two chips, one as the main processing unit, second as USB-to-serial converter.[[20]](https://arduino.stackexchange.com/questions/24081/is-atmega328p-the-same-as-16u2)
Arduino UNO rev 3 is the most recent version of the basic Arduino USB board.
It is based on ATmega328P processiong unit, but compared to previous version (Duemilanove) uses different USB-to-serial chip known as ATMega8U2 [[21]](https://www.arduino.cc/en/main/boards).
Arduiono duemilanove is since may 2009 based on same processing unit ATmega328P as its ancestor, no information about USB-to-serial chip found [[22]](https://www.arduino.cc/en/Main/ArduinoBoardDuemilanove).
Most of the "compatible" versions of Arduino UNO rev 3 uses CH340G chip instead of the ATMega8U2/ATM16U2.
As mentioned on quora [[23]](https://www.quora.com/What-is-the-difference-between-Arduino-Uno-R3-compatible-board-ATmega328P-ATmega16U2-and-Arduino-Uno-R3-ATmega328P-USB-board-CH340G-Which-should-I-buy-and-why) it should not be a problem, as far as installing software from the chineese manufactuer site is ok for the user. Another anwers mentioned additional coplications using board with CH430G instead of ATM8U2/ATM16U2.

**Sources**:  
[[20]](https://arduino.stackexchange.com/questions/24081/is-atmega328p-the-same-as-16u2) Is ATMEGA328P the same as 16U2? at _Arduino Stack Exchange_  
[[21]](https://www.arduino.cc/en/main/boards) Arduino Older Boards by _Arduino_  
[[22]](https://www.arduino.cc/en/Main/ArduinoBoardDuemilanove) Arduino Duemilanove by _Arduino_  
[[23]](https://www.quora.com/What-is-the-difference-between-Arduino-Uno-R3-compatible-board-ATmega328P-ATmega16U2-and-Arduino-Uno-R3-ATmega328P-USB-board-CH340G-Which-should-I-buy-and-why) What is the difference between Arduino Uno R3 compatible board ATmega328P ATmega16U2 and Arduino Uno R3 ATmega328P USB board CH340G? Which should I buy and why? at _Quora_

### 4. Approximate costs

After choosing non-presurized drip irridation system, it is required to barinstorm about required items and price them, before deciding whether this project is feasible.

Following items requires price estimation:
- Arduino board:
   - Arduino UNO R3 MEGA328P + CH340G
     - [AliExpress](https://www.aliexpress.com/item/32768431306.html) no cable 66.58+11.23 CZK at 26/06
   - Arduiono UNO MEGA328P + ATmega16U2
     - [AliExpress](https://www.aliexpress.com/item/32964588171.html) no cable 103.30+10.72 CZK at 26/06
     - according to comments works perfectly with Arduino software
   - Arduino NANO MEGA328P
     - [AliExpress](https://www.aliexpress.com/item/32309876432.html) Nano V3.0 FT232 by **Yanwen Economy Air Mail** 96.93+16.07 CZK at 26/06
     - [AliExpress](https://www.aliexpress.com/item/32309876432.html) Nano V3.0 CH340 by **Yanwen Economy Air Mail** 58.67+16.07 CZK at 26/06
   - Arduino MICRO MEGA328P
     - [AliExpress](https://www.aliexpress.com/item/4000160120491.html) **Pro Mini 328P-AU 5V** 48.21 CZK by **Yanwen Economy Air Mail**  at 26/06
     - [AliExpress](https://www.aliexpress.com/item/4000160120491.html) **CP2102 Micro USB** 25.26 CZK at 26/06
  - Nano terminal adapter
     - [Ebay](https://www.ebay.com/itm/Nano-Terminal-Adapter-for-the-Arduino-Nano-V3-0-AVR-ATMEGA328P-AU-Module-Board/133302815395) 39.66 CZK   
- Arduino Kits:
  - Elego UNO Project The Most Complete Starter Kit
     - [AliExpress](https://www.aliexpress.com/item/32638892215.html) 833.54 CZK at 21/06
     - mentioned in article about starting kits [here](https://makeradvisor.com/best-arduino-starter-kits/)
  - OR 
    - [AliExpress](https://www.aliexpress.com/item/32620337494.html) **DIP UNO R3** 615.21 CZK at 13/06
  - Sensor Kit  
    - [AliExpress](https://www.aliexpress.com/item/32592140121.html) 344.34+29.59 CZK

- Pipe-like components:
   - thin hose 4/7 mm 
      - [AliExpress](https://www.aliexpress.com/item/33052237739.html) 25m 237.21 CZK at 21/06
   - thick hose 16 mm
      - [AliExpress](https://www.aliexpress.com/item/4000618853699.html) 15m 343.57 CZK at 16/06
      - [AliExpress](https://www.aliexpress.com/item/4000732232580.html) 15m 404.28 CZK at 16/06
   - drip emmiter
      - [AliExpress](https://www.aliexpress.com/item/32912594761.html) 100pcs 256.09 CZK at 21/06
   - ziptie 3x200 (100pcs)
      - [AliExpress](https://www.aliexpress.com/item/4000094753931.html) black 49.23 CZK at **17/07**
   - ziptie 3x150 (100pcs)
      - [AliExpress](https://www.aliexpress.com/item/4000983441033.html) 3x150 **Yawen Economic Air mail** 35.20 CZK at 26/06
   - [PERSONAL] cable ties (50pcs)
      - [AliExpress](https://www.aliexpress.com/item/4000843570179.html) 82.39 CZK
   - [OPTIONAL] Hoop pipes (10pcs)
      - [AliExpress](https://www.aliexpress.com/item/10000150195823.html) 10-16mm 43.11 CZK
- Electronics valves:
   - 12V DC 1/2" Plastic Solenoid Valve
      - [AliExpress](https://www.aliexpress.com/item/33019875310.html) DC 12V **Yawen Economic Air mail** 81.88+5.36 CZK at 26/06
- Arduino required sensoric equipments:
   - Postponed    
- Water container:
   - IBC NÁDRŽ 1000L
   - About 3000 CZK, with VATS and cage
   - **Recommend ask uncle/cousin for seller**
- Pumps: 
   - Posponed


| Item  | Prices | Links | Notes  |
|-------|--------|-------|--------|
| Valve |        |       |        |
| Pump  |        |       |        |
| Board |        |       |        |

