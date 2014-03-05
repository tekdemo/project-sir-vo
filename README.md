SirVo Project
=============

A servo motor replacement board that runs a magnetic encoder for continuous rotation without loss of tracking. 
Runs the Arduino environment on an embedded Atmega 328, exposing hardware PWM capture, I2C, and UART to a 4 wire input cable. 

Additionally, allows for a header on the back of the motor controller, with the intention that you could include "backpacks" that extend the functionality much like you do with an Arduino Shield. 

Uses OpenServo board footprint, which should fit some medium size servo controllers

Currently in the testing phase, with several known flaws in the hardware


Known Bugs
============

- Forgot the pulldown resistors on the mosfet driver

- Code still very unfinished (and hence, not posted). 

- Motor slot alignments are incomplete, and need testing

- Following OpenServo's wiring scheme is not ideal, breaking compatibility with their leads will improve routing and logical wiring hookups

-Attempted a hacked in multiplexing scheme for the I2C and UART lines, and have not determined that either of them work as expected. 







