# MQ135
This is an Arduino library for the MQ135 gas sensor. Its purpose is to provide estimate concentration of CO2 in the air surrounding the gas sensor, in units of ppm.

Main features of the library:
*	Automatic baseline calibration, meaning the sensor is automatically calibrated on the fly. Note that the baseline is not stored in the NVM, therefore it is lost after an Arduino reset.
*	No need to define the load resistor’s value.
*	Temperature and humidity compensation of the CO2 readings.
*	Contains option to select between two manufacturers of the MQ135, Winsen and Olimex.

The library was created with these environmental assumptions in mind:
*	The sensor will be used in a typical home or office indoor environment. Such environment contains low-to-no concentration of gases other than CO2 to which the MQ135 responds (e.g. ammonia, toluene).
*	The sensor will be used in an indoor environment that is well ventilated at least once per week.
*	The CO2 concentration of the outdoor environment is about 400 ppm.
