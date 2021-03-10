# DSI DataBase Fan

This project was created for the mexican company Software DSI.

The aim is to controll the fans that cool the database room with a microcontroller.
It works in the following way:
It has a defined temperature in which the fan will be turned on (this value can be changed by the users) and another defined temperature in which the fan will be turned off (also a value that can be changed by the users).
So, when the room temperature goes above the turn on temperature value, the microcontroller activates the fans. And, after a while, when the fans have done their work and the temperature has gone below the turn off temperature value, the microcontroller shuts down the fans.

This projects consists of two parts:

1.- C code for the microcontroller.
This is the code that tells the microcontroller what to do. It needs to be compiled with a program that can produce the files that we actually upload to the microcontroller. Like the .hex file also included in this project.

2.- Proteus simulation.
To probe that the program as well as the electronic schematics is ok, a proteus simulation was created. An image of the running simulation is showed below. To run the proteus simulations, the .hex file is needed.

![proteus simulation](https://github.com/CamilAbraham/DSI_DataBase_Fan/blob/main/ProteusSimulation.PNG?raw=true)

As we can see, there are:
Four buttons, which can be used to change the turn on and turn off temperature values. 
An LCD display that shows the current on/off temp values, as well as the current humidity and temperature in the room.
The microcontroller that controlls everything, and a crystal which is needed by every microcontroller to work.
An DHT22 sensor, which is the one that measures the room temp.
And a led, which simulates the fan.  When the led is on it represents the moments when the fans are activated, and when its off the fans are turned off.
