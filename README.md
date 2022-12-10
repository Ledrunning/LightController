# LightController

### Open source project to control light in the room, garage, street, house etc;

* In this project, I used a small Atmel AVR microcontroller Attiny13A, Pir sensor HC-SR501,

and handmade opto driver (light sensor based on a phototransistor and Rail-To-Rail OP mcp6021);

* The program is written in C language in Atmel Studio 7 IDE;

* In the PCB folder you can find schematic circuits and PCB;

* In the LightController folder you can find the source code and the Atmel Studio project;

* In D3MG_PCB folder you can find PCB for DIN-rail package D3MG;

* In the Simulation folder you can find Proteus 8 project file for device simulation;

* In the FUSEBIT_scr folder are screenshots with fuse bits configuration from the Khazama programmer;

* In the BOM folder you can find the BOM(bill of materials) of the main board and photo driver;

Algorithm:
Priority always has a light key switch, regardless of the level of illumination of the object and when the PIR sensor is active.

After about 5 hours, when the light key switches on, the light will automatically turn off.

If the light key switch is turned off, and the object is in the PIR-sensor zone and dark outside, the light turns on and stays until the object leaves the field PIR-sensor.

If the light key switch is turned off, the object is in the PIR-sensor field and dark outside, the light is turned on and lights up when the subject in the field of PIR sensor lighting continues to work for about 300 seconds.

If the light key switch is turned off, the object is in the PIR sensor and the street light does not turn on until the light level drops below a predetermined threshold or switch on a light.

# Prototype photo: 

<img src="https://habrastorage.org/files/e9f/563/888/e9f563888cdf4c149a052febf3b871ff.jpg"/>

# Conections: 

<img src="https://habrastorage.org/files/5c6/6e2/3ce/5c66e23ce82f4ff2a964b5d229b054eb.jpg"/>

More informations in Russian - https://ledrunning.wordpress.com/2017/01/05/garage-light-controller/ (You can use the gtranslate on this site on right corner or on bottom(basement) of main page).

Hackaday - https://hackaday.io/project/169694-light-controller
