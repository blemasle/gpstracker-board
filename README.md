# High autonomy GPS tracker.

A custom Arduino 2 layers board meant to be use with a dedicated [firmware](https://github.com/blemasle/arduino-gpstracker). The result is a high autonomy GPS tracker that can be use to track moving vehicules.

See the [firmware repository](https://github.com/blemasle/arduino-gpstracker) for more info.

## Hardware
This project has been build on a [ATMega328p](https://www.microchip.com/wwwproducts/en/ATMEGA328P) for its ease of use, low power consumption and wide support.

On top of that, several ICs are needed :
* [SIM808](https://simcom.ee/documents/?dir=SIM808) : GPRS & GPS.
* [DS3231](https://www.maximintegrated.com/en/products/digital/real-time-clocks/DS3231.html) : Real Time Clock, used for time keeping and battery saving.
* [24LCxxx](https://www.microchip.com/wwwproducts/en/en010828) : EEPROM used to buffer raw data before sending.

## Soldering
Solering this circuit board requires either the use of soldering paste or fine soldering skills. 
The SIM808 IC can indeed be quite hard to solder by hand because of its form factor that requires you to solder each one of its 64 pins separately instead of the usual flux and drag technique.   Moreover, the shape of each pin make it very easy to solder several pins together or soldered with not enough tin to make a reliable connection.