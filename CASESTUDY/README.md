![Smart watch](https://user-images.githubusercontent.com/98769359/154833030-d8d4f189-ec24-4c48-a63c-608147739f96.png)

## Push button(power up)
The push button is used  to turn the device on and off and can be used even to restart the watch .

## Voltage regulator
The voltage regulator can connect the supply voltage divided output from the IC directly to the A/D converter of the low-voltage microcontroller, allowing the microcontroller to monitor the battery voltage without a divider resistor.

## Controller
The controller controls the various functions on the watch such as step mesaurment temperature sensor etc, and diverges the data to the memory chip for storing and this data can also be displayed on the LCD display.

## Bluetooth
The bluetooth establishes a connection between the watch and the device which it is connected with which is gnereally a samrtphone and we can also access the features of the watch through an application within the smartphone .

## LCD
The LCD display acts as an output for the all the inormation that is given out by the different sensors . 

## Memory chip
The memory chip stores all the data from all the sensors that is processed and btought in by the converter.
It also stores the time , date and other general information .

## Heartbeat mesaurment sensor
Heart beat mesaurment sensor uses infrared rays to mesaure the pulse and give the output in the form of a particular number .

## Blood pressure monitoring 
In blood pressure monitoring optical sensors  check if vessels are tightening or widening. An algorithm then uses those two bits of information, along with heart rate, to estimate blood pressure .

## Accelerometer 
Accelerometer detects movement and tracks direction . It is the most common sensor that you will find inside a wearable. This sensor can track forward and backward movement, sense gravity and determine body's orientation, position and also rate of speed change.

## Temperature sensor
A temperature sensor  detects and measures hotness and coolness and converts it into an electrical signal.

## Humidity sensor
How does the humidity sensors work?
Humidity sensors work by detecting changes that alter electrical currents or temperature in the air.  Two thermal sensors conduct electricity based upon the humidity of the surrounding air. One sensor is encased in dry nitrogen while the other measures ambient air. The difference between the two measures the humidity.


## High level requierments
|ID|specification|
|--|--|
|HR 01|User shall be able to turn the watch with push button|
|HR 02|User shall be able to turn the display on when watch is tilted.|
|HR 03|User shall be able to mesaure the number of steps walked|
|HR 04|User shall be able to see the current room temperature|
|HR 05|User shall be able to monitor blood pressure and herat beat|
|HR 06|User shall be able to connect the smart watch with smartphone through bluetooth|
|HR 07|User shall be able to read notifications of his smartphone on the display of smartwatch .|

## Low level requierments
|ID|Specification|
|--|--|
|LR 01|The push button must be pressed for 5seconds to turn on the watch|
|LR 02|To turn on the display of the watch it must either be tilted or double tapped on thje screen.|
|LR 03|Step counter must be able to detect the motion in order to count the number of steps walked .|
|LR 04|To mesaure blood pressure user must turn on the blodd pressure monitoring system .|
|LR 05|To mesaure heart beat user must turn on heart beat sensor .|
|LR 06|To read notifications from the watch user must turn on bluetooth and sync the watch with the app and turn on notification setting .|







