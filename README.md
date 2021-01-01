# Mode S plugin

This plugin was designed to simulate mode S correlation on EuroScope, for use on the VATSIM Network. Just load the plugin in EuroScope, and squawk 1000 will be assigned for capable aircraft above FL245 without assigned sqauwk or with generic codes like 0000, 1200, 2000, 2200.
Manual assignment is available for all applicable aircraft and aircraft on ground.

The plugin needs the Visual C++ Redistributable for Visual Studio 2015. If you have trouble to load the plugin, install it from here: https://www.microsoft.com/en-us/download/details.aspx?id=48145

## Available tag items

* Transponder type: Show wether the aircraft is mode S or not
* Mode S: Reported Heading: Reported magnetic heading of the aircraft
* Mode S: Roll Angle: Reported roll angle (L for LEFT and R for RIGHT + value in degrees)
* Mode S: Reported GS: Reported groundspeed of the aircraft in knots.

## Available tag functions

* Assign mode S squawk - assigns code 1000 to aircraft with mode S transponder
* Assign mode S/A squawk - same as above, but opens the default assignment popup for aircraft without mode S transponder (meant to be used in the EuroScope lists).

## EuroScope set up
* Load up the plugin
* Set your mode S string to ```HLEGWQS```
* Add ```1000``` to your VFR squawk list (to prevent squawk duplicates)
* Set the "Mode S Plugin / Assign mode S/A sqauwk" function to replace the default
* Allow the plugin to draw on all types of radarscreens
![Tag Setup](http://cherryx.de/modes/modespluginlist.png)
![Plugin Setup](http://cherryx.de/modes/modesplugin.png)

## Add a country to the mode S list

If you would like to add a series of airports to the mode S, create an issue on this GitHub with your request, you can see all the currently enabled areas in the file "version.txt"

The current mode S airspace for the plugin is as follows:

![Mode S Map](https://camo.githubusercontent.com/b55cdc532e8344ecee7ca2a6dec2c6b127fbe358b9ce60da1176bc5d7db8bddf/68747470733a2f2f692e696d6775722e636f6d2f305655684d61642e706e67)
