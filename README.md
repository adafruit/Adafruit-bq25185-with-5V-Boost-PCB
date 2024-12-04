## Adafruit bq25185 USB - DC - Solar Charger with 5V Boost Board PCB

<a href="http://www.adafruit.com/products/6106"><img src="assets/6106.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit bq25185 USB - DC - Solar Charger with 5V Boost Board. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6106

### Description

We're always on the look out for better ways to make projects portable: being able to charge your battery in the most convenient manner will let projects run no matter what power is available. Then we added a power supply chip with it to let you run your project without a separate board. The result is the Adafruit bq25185 USB / DC / Solar Charger with 5V Boost Board!

It uses the new bq25185 is a nifty charger chip with fairly high charge current, power path support, and the ability to charge from USB, DC or solar power. It's also a great value, so it's a good upgrade from MCP73833 or MCP73831-based charger boards. The boost converter is the TPS61023, which will give up to 1 Amp output with good efficiency, to squeeze the most power possible out of your battery.

This board is meant to be everything you need to power your 5V electronics: simply connect a 500mAh or larger battery to the JST PH 2-pin port, then charge it when you can from USB or DC/solar. At the other end is a terminal block which will provide the 5V output from the boost converter. 

* USB Type C connector with 5.1k CC resistors so it will work with any computer or power supply to get 5V and up to 1A. Data lines available if needed, on the bottom breakout.
* Separate DC or Solar Input - Two pads on the edge can be used to connect a 5 ~ 18V power supply, which can be used instead of USB. If the input is a solar panel, the charging chip will adjust the current draw so that the voltage does not dip below the battery, thus optimizing the solar power input. No large capacitor needed to stabilize it, and you get near-MPPT capability without the cost and complexity of MPPT.
* Default charge rate of 1A, but you can cut the jumper on the back to set the rate to 500mA
* Power Path to Load - If the 5V load connector is drawing current while the USB / DC/Solar power is attached, it will default to drawing current from the charger and any left over current will go to the battery. That keeps your battery from constantly charging/discharging which will reduce the battery life.
* Regulated 5V Output - a boost converter will take the load output from the bq25185 and convert it to 5V at 1 Amp max load. Note the TP61023 cannot turn on/off high loads, it will stall over 200mA. That means its not going to like it if you have a high current load that instantly draws full current on power up, like a resistive dummy load. The vast number of microcontroller projects will start up with <200mA and then a half second later will turn on high current items like LEDs, motors, wifi/radios, or displays so the restriction won't affect it.
* Three Status LEDs - Orange Charging LED, red Fault LED, and Green 3.3V output LED.
* Enable pad - to disable the 5V boost converter.
* Mounting holes!

This board is pretty much plug-and-play. Change the charging jumper if you like, then connect your battery to the BATT port, and the 5V output goes to your circuit. You can monitor the voltage on the battery via the secondary pads on the bottom edge, if necessary.

To use with solar, pick up a 5~7V solar panel (using a higher voltage panel will only lose the extra voltage as heat so there's no benefit to going over 7V), and either cut the connector off to wire it directly, or use a 2.1mm adapter cable plus a 2.1mm terminal block to get two wires for the DC Input port.

If you need a board with higher charge current or a DC plug already on-board, check out the bq24074 which has up to 1.5A charge rate and a on-board 2.1mm DC jack. It doesn't have a boost converter but you could wire up the TPS61023 separately

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
