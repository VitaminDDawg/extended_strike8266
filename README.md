# extended_strike8266 V0.1
## Esp8266 Wifi Range extender with rogue external dns capabilities

## Discription:
This esp8266 arduino sketch allows your device to connect to the network of your choice acting as a wifi range extender with
the option to choose your own external dns server(dnschef). This is useful for traffic analysis and everything
useful about having full dns control of a network without the need for network exploitation, mobile internet or a device such as a wifi
pineapple. At $0.50-$2.00 per unit this is the absolute cheapest option for evil twin attacks.

## ToDo:
- [ ] add dns option to web interface

- [ ] add captive portal options

- [ ] fix bugs

- [ ] pretty up web interface

- [ ] esp hosted local dns rules?


## Requirements:
esp8266 board

arduino-ide

arduino esp8266 board libraries

## headingSetup:
1)paste or open the extended_strikev0.1.ino sketch in the arduino-ide

2)setup your dns server (dnschef server "https://github.com/iphelix/dnschef")

3)add your dns server ip address to the script manually (line 51. The default is "8, 8, 8, 8")

4)upload/flash your sketch to your esp8266

## Connection setup:
1)after upload the device will reset and create an open wifi network called "farylink"

2)connect your phone or computer to the open network "farylink"

3)in your browser go to http://172.217.28.254 to setup your wifi options
(when you load "http://172.217.28.254" the device scans for networks around you)

4)the first options include the names of the networks it has scanned. Select your target network
if it is an open network leave the password field blank

5)click "apply" (this will disable the connection temporarily)

6)wait for the "fary" network to reappear in your wifi settings.

7)when it reappears it should be connected to your target network

8)if you would like to change your ESPs network broadcast name or add a password reconnect, go
back to http://172.217.28.254 and modify the fields to your choosing.

## Do not use this on networks you do not own or have permission to use. follow all applicable state and federal laws. Thank you, happy hacking.
Range extender code shamelessly stolen from somewhere.
