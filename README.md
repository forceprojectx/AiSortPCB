# AiSort Arduino
Features connectors which match the parts list with the exception of the proximity sensor which does not include a connector.
Uses bluetooth for pc connectivity because I am big dumb and forgot that the webcam needs to plug in, so it can't be a fully wireless connection.

## Microcontroller
Uses Arduino pro mini as controller 

## Motor Drivers
supports both the TCM 2209 and DRV8825 motor controllers. You can use a matched pair or mix and match, based on what components you have on hand.

## PC Connectivity
The AiSort board is designed to use HC-05 bluetooth modules for PC connectivity. If your PC does not have bluetooth, you may connect a USB-UART device to the pins labeled `TX0` and `RXI`  on the microcontroller or connector J2. 
`TXO` is connected to `J2.1`  
`RXI` is connected to `J2.2`  
`GND` is connected to `J2.8`  
`VCC` is connected to `J2.7`  

## Fan Connectors
Features 3 fan connectors. Two standard 3 pin fan connectors (KF2510-3P) and one 2 pin JST XH type connector. 

## External Trigger Out
The board has two ports to connect external 12volt triggered devices. These are KF2510-2A connectors as found here [KF2510 Connector Kit](https://www.amazon.com/dp/B01M69TKAM)
These triggers can be used to trigger the air solenoid or a round counter or whatever.
> Only one is currently functional due to the limited pinout of the arduino pro mini.

## Proximity Sensor
Unfortunately the proximity sensor does not come with a default connector.
The board is designed to use a JST XH-5A. It is 5 pin only to ensure it does not mate with the other connectors on the board such as the homing sensors. Pin 3 is the signal pin. Power and ground pins are doubled so you can use either of Pins 1 and 2 for ground and either of Pins 4 and 5 for +12v. 
If you have a soldering iron, you can just solder the wires directly to the board if you dont have the appropriate connectors and crimping tools.

