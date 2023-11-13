# ThermistorTrigger
Setpoint trigger designed to be a hardware failsafe for thermistor based temperature readings

This is designed to be a trigger board that can trigger other devices in the event of an overtemperature.  

Simply plug a standard thermistor into either input then the signal is buffered by an opamp and stabilized.  From there you can take the signal out and send it to your main control board as a temp sensor but it also drives into another opamp setpoint trigger which is set by the onboard potentiometer.  This allows you to set a trigger point in hardware that will drive the digital output of the setpoint trigger low if it exceeds the desired temp.

This is intended to go along with a couple of my other projects (Flambehub and Flambegate which are the devices which will kill the power in a "dumb" way requiring no MCU intervention) but this can also be used on a device such as a 3d printer (or other CNC device) to trigger a halt on the MCU if it is attached to the control board.
