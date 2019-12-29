# thermostat
wifi enabled thermostat, everything open source

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
* MCP9809? - high precision temperature sensor, I2C
* DS3231? - real time clock
* Omron G6AK-247? - 2 coil latching relay, 3V
* TFT screen?

## Failsafe
We don't want frozen pipes if the unit fails
* watchdog timer?
* regular thermostat in paralell?

## Schematic and PCB layout
* Eagle PCB will be used, files will be available online
* Bare boards will be available to anyone that wants one
