# LightController

### Open source project to control light in the room, garage, street, house etc;

* In this project I used small Atmel AVR microcontroller Attiny13A, Pir sensor HC-SR501,

and handmade optodriver (light sensor based on phototransistor and Rail-To-Rail OP mcp6021);

* The program written on C language in Atmel Studio 7 IDE;

* In PCB folder you can find schematic circuits and PCB;

* In LightController folder you can find source code and Atmel Studio project;

* In D3MG_PCB folder you can find PCB for DIN-rail package D3MG;

* In Simulation folder you can find Proteus 8 project file for device simulation;

* In FUSEBIT_scr folder are screen shots with fuse bits configuration from Khazama programmer;

* In BOM folder you can find BOM(bill of materials) of main board and photodriver;

Algorithm:

Priority always have a light key switch, regardless of the level of illumination of the object and when PIR-sensor is active.

After about 5 hours, when the light key switch on, the light will automatically turn off. 

If the light key switch is turned off, and object is in the PIR-sensor zone and dark outside, the light turns on and stays until the object leaves the field PIR-sensor.

If the light key switch is turned off, the object is in the PIR-sensor field and dark outside, the light is turned on, and lights up when the subject in the field of PIR sensor lighting continues to work about 300 seconds.

If the light key switch is turned off, the object is in the PIR-sensor and light street light does not turn on until the light level drops below a predetermined threshold or switch on light switch.

# Prototype foto: 

<img src="https://habrastorage.org/files/e9f/563/888/e9f563888cdf4c149a052febf3b871ff.jpg"/>

# Conections: 

<img src="https://habrastorage.org/files/5c6/6e2/3ce/5c66e23ce82f4ff2a964b5d229b054eb.jpg"/>

More informations in Russian - http://ledrunner.ru/2017/01/05/light-controller/ (You can use the translate in this site on top right corner)
