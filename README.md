# MySecurity
Integrate existing alarm system into my smart home ecosystem

Integration into an existing security system is doable.  In my situation, I wanted to leverage my existing window and door sensors.  These sensors are all pulled back to an alarm panel in my master closet (must be a standard thing builders do).  My first attemp was to just wire up open/close sensors that were zwave.  These work fine but can be too clostly for most @ $25.00/each.  This is my second attemp to make things cheaper but scale for any size home.

To the devices & Smartthings.

You will need a few things to get this to work.  
 1) Smartthings app located here (optional) (free)  
 2) Virtual device (free)  
 3) Arduino and code ($35 for the original but 3rd party $8)  
 4) Smartthings Shield (https://shop.smartthings.com/#!/products/smartthings-shield-arduino) ($35 bucks ouch)  
 5) Arduino kit ($14 just an easy way to prototype stuff)  
 6) Reed sensors ($1 each)  
 
 You can see the working solution here: https://www.youtube.com/watch?v=Z47ct-1E8KQ
 
 
 Wiring up the Arduino  
 
 You'll need to update the Arduino code for the pins you want to use but this demo uses pins 9, 10, & Ground.  Wire up on end of the first reed sensor to pin 9 & the other second wire to ground.  Wire up the second reed sensor to pin 10 and the second wire to ground.  No resister is required in this case because we are going to use the internal resister.
 
 Joining the Arduino  
 Go ahead and join the arduino to smartthings.  At this point, its just doing a regular join by using the smartthings app.
 
 In Smartthings API  
 Go in and create your device handler using the file included above called "virtual device".  Save it and publish it.
 
 Assign the device type to the Arduino  
 Going back to your devices, you need to find the arduino you just added.  Once there, edit the device and change the device type to the name of your device handler.
 
 At this point, you should be able to test the security device and see the reed sensors light up your phone.  If you don't, then you should stop and go back over the directions.


 
 
 
 
