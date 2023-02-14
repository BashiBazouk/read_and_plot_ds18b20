# Read from DS18B20 sensor and plot live data in python
**_Work in progress_**

Idea of project is as always: learn python, C++ for arduino and some electronics. End result may be useful in some future for complex, integrated layout of different sensors, to measure situation.

## Sources
Basic start of this project for me was, but it's in polish:<br>
[Jak podłączyć i programować termometr cyfrowy DS18B20 w Arduino PL](http://akademia.nettigo.pl/ds18b20/)
similiar in EN:
[Interfacing DS18B20 1-Wire Digital Temperature Sensor with Arduino ](https://lastminuteengineers.com/ds18b20-arduino-tutorial/)
## How it works?
There are three parts of this project:
- Hardware (excluding Arduino)
- Code for Arduino in C++
- Script in Python 

**Hardware** is responsible for taking measurements. It's very simple assembly based on I2C sensor [DS18B20](https://www.elprocus.com/ds18b20-temperature-sensor/). It's ideal for use for home appliances, easy to use, energy saving and cheap.
I2C means that wiring is basically wires and one resistor. On single line thare can be many sensors.
TODO:
- [ ] add (many) more sensors and test it

**Arduino code** is responsible for initiating communication with DS18B20, reading from sensor, and sending data thru serial to PC
TODO: 
- [ ] change code so measurement is done when there's request from serial port, and then sent measurement

**Python Script** is responsible for reading from serial port, and displaying data on diagram
TODO: 
- [ ] script has to send request, and then plot new data on diagram
- [ ] make sure diagram (diagrams?) are clear when many sensors are used


## Build
Assembly diagram:<br>
![ds18b20_single.png](diagram)<br>
Ready breadboard and arduino:<br>
![1676229289947.jpg](breadboard)<br>
