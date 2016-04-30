## Talky-plant: a sensor connector for esp-8266 NodeMCU v3

Board files for my ongoing project to create internet-connected sensors. For
the ESP8266 code, see [extra sensory](https://github.com/RLuckom/extra-sensory)

This is a kicad project containing a board layout for a daughterboard to connect 
the NodeMCU v3 board to a DHT11 temperature / humidity sensor, a YL-69 soil 
moisture sensor, and a photoresistor to measure sunlight levels.

TODO:

1. The resistor values listed in the schematic don't take into account either
   the voltage drop across the diodes or the values resistors actually come in.
   The resolution is way below what should be possible and I don't see the full
   range of adc values from either photoresistor or YL-69.

2. Everything I've read suggests that soil moisture sensors are extremely
   short-lived devices. I have to characterize them better, and in the hardware
   design I should plan for having to switch out the fork part that goes in the
   soil.
