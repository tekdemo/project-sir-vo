SirVo Project
=============

A servo motor replacement board that runs a magnetic encoder for continuous rotation without loss of tracking. Runs the Arduino environment on an embedded Atmega 328, exposing hardware PWM capture, I2C, and UART to a 4 wire input cable.

Additionally, allows for a header on the back of the motor controller, with the intention that you could include "backpacks" that extend the functionality much like you do with an Arduino Shield. 

Uses OpenServo board footprint, which should fit some medium size servo controllers. Tested on Parallax Continuus Rotation Servo, and looks like it should fit TowerPro MG995 servos (which require modifications for continuous rotation).

Currently in the testing phase, with several known flaws in the hardware


Known Bugs
============

- H bridge needs a proper driver for operation with higher input voltages. 

- Voltage regulator isn't performing satisfactorially, and needs to be replaced. Currently requires external 3.3V supply to function.

- Code still very unfinished (and hence, not posted). The exception is the [AS5050 Library](https://github.com/tekdemo/AS5050), which is reasonably functional.

- Motor slot alignments are still not known to function on all brands of servos, but work well for now.

- This uses a very strange passive multiplexing scheme I hacked together for the I2C and UART lines. It's been confirmed to work for UART data transmissions, but I2C is still untested. 







