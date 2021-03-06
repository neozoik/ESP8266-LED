## Hardware setup

The ESP8266 comes in different versions. They differ slightly in pin layout, more information is available [here](http://www.esp8266.com/wiki/doku.php?id=esp8266-module-family).

I'm using the ESP-12F, which needs the following connections:

![Pin configuration](https://github.com/christophhagen/ESP8266-LED/blob/master/esp12F_connections.jpg)

[Image source](http://www.instructables.com/id/Getting-Started-with-the-ESP8266-ESP-12/step3/Make-the-connections/)

Note that `GPIO0` needs to be low only upon power up to boot into flashing mode (to upload code). Have it high/floating to boot the device into normal operations.

You can use any available pins for the data/clock lines of the LED strip, just specify the ones you used in the `parameters.h` file.
