# MySecurity
Integrate existing alarm system into my smart home ecosystem

Integration into an existing security system is doable.  In my situation, I wanted to leverage my existing window and door sensors.  These sensors are all pulled back to an alarm panel in my master closet (must be a standard thing builders do).  My first attemp was to just wire up open/close sensors that were zwave.  These work fine but can be too clostly for most @ $25.00/each.  This is my second attemp to make things cheaper but scale for any size home.

To the devices & Smartthings.

You will need a few things to get this to work.
 1) Smartthings app located here (optional)
 2) Virtual device
 3) Arduino and code
 4) Smartthings Shield
 
 You can see the working solution here: https://www.youtube.com/watch?v=Z47ct-1E8KQ
 
 
 Wiring up the Arduino
 
 You'll need to update the Arduino code for the pins you want to use but this demo uses pins 9, 10, & Ground.  Wire up on end of the first reed sensor to pin 9 & the other second wire to ground.  Wire up the second reed sensor to pin 10 and the second wire to ground.  No resister is required in this case because we are going to use the internal resister.
 
 
 
 
