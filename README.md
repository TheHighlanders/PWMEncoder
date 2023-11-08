# A Custom PWM Encoder for FRC
This encoder connects to a SparkMAX Motor Controller, using the Data Port. This encoder was designed with use on Swerve Drive Specialties Mk 4 Modules, with NEOs. 

These utilize the AS5047 chip to read a rotating magnetic field, and convert that to a PWM output.

Included in this repo are the KiCAD project files, as well as STEP file for the board, and 2 parts of a case that we used to mount these encoders.

## Important Notes

### Data Port Connector
In the project files, the Data Port connector is included on the incorrect side of the board. The pinouts for the board are correct, the only change that needs to be made if you use these is in assembly, the connector should be mounted on the top side (with the LED) of the board, and the notch should face away from the encoder IC.

### Programming the IC
The AS5047 encoder used here requires a programming process to output a PWM signal. A script to do this via an Arduino can be found here: [Programming Script](https://github.com/TheHighlanders/AS5047ProgrammingScript)