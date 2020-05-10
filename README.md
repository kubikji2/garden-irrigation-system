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
 

