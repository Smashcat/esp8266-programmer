# esp8266-programmer
Eagle files for a small ESP8266 programmer with auto-programming mode/reset

This uses mostly SMD parts, so really needs to be cooked in an oven or hotplate due to the density (difficult to get an iron into the right places). I've also included the library part for the USB port, as I found the version online (at Octopart) has an incorrect footprint. I ordered 10 of these, plus a stencil from JLCPCB at a cost of $8, plus shipping! I would suggest getting the stencil if you intend to make a few, as it saves a ton of time, and makes the board look a lot cleaner.

The board can supply around 400mA of current at 3.3v, so should easily be able to power an ESP8266 module, with plenty to spare for other components such as an LCD etc if needed. If you're already powering the ESP from another source, then do not connect the 3v3 pin from the programmer.

There are LEDs on each of the active pins, plus 3v3, so you can see activity at all times. It also means that it's possible to control the LEDs on the programmer via the GPIO0, RX and TX pins on the ESP if you like (pull them low to light the LED). The LEDs and their resistors are optional - the programmer will still work without them.

![Programmer](http://www.smashcat.org/av/esp_programmer.jpg)
