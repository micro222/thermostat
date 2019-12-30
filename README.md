# wifi enabled thermostat, everything open source

## Server
* adafruit.io?
* provide its own server?
>"You can have it as it's own server if you use port forwarding from your router and use the IP address of your provider.
>Or
>register a domain to your home (with a static IP, or you can run software in your router to report your IP to the name service)...
>Or
>you can have it somehow call out the IP address to your phone if it's not dynamic...I think most people don't have have a static IP in their home.. so you could depend on running DDWRT or something in your router.. or make your own similar service in the device."   -Darcy

>"you could forward ports from your modem/firewall to your device (for direct access), but that leaves you open to the possibility of someone externally poking at it.  (aka hacking)"   - Justin

## Parts
* ESP32?  what board? ESP32 thing?
>I like the Lolin32 LITE... It has a small footprint, the same I/O as its larger siblings and is very cheap! - Adrian
* MCP9809? - high precision temperature sensor, I2C
* DS3231? - real time clock
* Omron G6AK-274P-ST-US-DC3? - 2 coil latching relay, 3V
* ULN2003 or MDC3105DMT1G?                                
* TFT screen?

## Failsafe
We don't want frozen pipes if the unit fails
* watchdog timer?
* regular thermostat in paralell?

## Schematic and PCB layout
* Eagle PCB will be used, files will be available online
* Bare boards will be available to anyone that wants one

## Other attempts at an ESP-based thermostat
* https://github.com/tomikaa87/esp-thermostat
* https://www.letscontrolit.com/forum/viewtopic.php?t=6287

## Things to do
* how do we set the time and date?

## Firmware
* regulate temperature
* show current temperature and setpoint on display and webpage
* store setpoints for the week
* allow editing of setpoints from a webpage
* indicate 
* allow switching between manual and programmed setpoints


## Front panel
For now we can control the device through a web page, but eventualy a screen and some buttons would be nice to have
What controls do we need?
* current temperature and setpoint
* burner status
* on hold or programmed
* time and date
