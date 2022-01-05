# MeteoBridge Plugins

## Wind Average Plugins

This plugin is usefull to compute wind speed average, in case the weather station do not compute it, like "Davis Emulator" from Anemos http://docs.anemos.ovh/acc-sens.html#emulator.

### How it work
The plugin work like a new (virtual) weather station that add a new wind sensor, collect wind data from primary weather station using the meteobridge cgi script every 5 seconds and compute the average over the last 120 samples (10 minutes).
Then return the last sample as wind gust speed and wind average speed on the added wind sensor (wind direction is 0 deg).

### Setup

1. Add a new wheader station
2. Setup the weather station as 'User-defined'
3. copy the file "windavg.plugin" on a webserver to be that it is reachable like the example provided by meteobridge.
4. Reload the Plugin
5. Save the configuration.
6. In Mapping page, remap the wind average sensor to the new wind average sensor.


### appendix
Special thanks to TrimbleSoftware (https://github.com/TrimbleSoftware): https://github.com/TrimbleSoftware/mbwbpi
Topic related on Meteobridge Forum: https://forum.meteohub.de/viewtopic.php?f=56&t=16149
MeteoBridge: https://www.meteobridge.com/wiki/index.php/Home
 

