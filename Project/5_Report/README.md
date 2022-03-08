## Distance Measurement using AVR Microcontroller And HC-SR04
## Introduction
In this project, we are going to use an HC-SR04 ultrasonic sensor to give your robot the perception of distance.This popular ultrasonic distance sensor provides stable and accurate distance measurements from 2cm to 450cm. It has a focus of less than 15 degrees and an accuracy of about 2mm.This sensor uses ultrasonic sound to measure distance just like bats and dolphins do. Ultrasonic sound has such a high pitch that humans cannot hear it. This particular sensor sends out an ultrasonic sound that has a frequency of about 40 kHz. The sensor has two main parts: a transducer that creates an ultrasonic sound and another that listens for its echo. To use this sensor to measure distance, the robot's brain must measure the amount of time it takes for the ultrasonic sound to travel.Sound travels at approximately 340 meters per second. This corresponds to about 29.412µs (microseconds) per centimeter. We know that sound vibrations can not penetrate through solids. So what happens is, when a source of sound generates vibrations they travel through air at a speed of 220 meters per second. These vibrations when they meet our ear we describe them as sound. As said earlier these vibrations can not go through solid, so when they strike with a surface like wall, they are reflected back at the same speed to the source, which is called echo. Ultrasonic sensor “HC-SR04” provides an output signal proportional to distance based on the echo. The sensor here generates a sound vibration in ultrasonic range upon giving a trigger, after that it waits for the sound vibration to return. Now based on the parameters, sound speed (220m/s) and time taken for the echo to reach the source, it provides output pulse proportional to distance. To measure the distance the sound has travelled we use the formula:

Distance = (Time x SpeedOfSound) / 2

The "2" is in the formula because the sound has to travel back and forth. First the sound travels away from the sensor, and then it bounces off of a surface and returns back.

The easy way to read the distance as centimeters is to use the formula:

Centimeters = ((Microseconds / 2) / 29).

## Component Requiered
Hardware: ATMEGA32, Power supply (5v), AVR-ISP PROGRAMMER, JHD_162ALCD (16x2LCD), 1000uF capacitor, 10KΩ resistor (2 pieces) , HC-SR04 sensor.

Software: VSCode, SimulIde, Ardunino

## 1.ATMEGA32
The high-performance, low-power Microchip 8-bit AVR® RISC-based microcontroller combines 32 KB ISP flash memory with read-while-write capabilities, 1 KB EEPROM, 2 KB SRAM, 54/69 general purpose I/O lines, 32 general purpose working registers, a JTAG interface for boundary-scan and on-chip debugging/programming, three flexible timer/counters with compare modes, internal and external interrupts, serial programmable USART, a universal serial interface (USI) with start condition detector, an 8-channel 10-bit A/D converter, programmable watchdog timer with internal oscillator, SPI serial port, and five software selectable power saving modes. The device operates between 1.8-5.5 volts.

## 2. AVR-ISP Programmer
Until now,Support IC manufacturer, pcs devices and keeps growing. High speed thanks to the flexible hardware engine. Programming speed adjustable for complicated application environments brought by user target board, length of ISP cable etc. Stand-alone and PC-Hosted (USB2.0 High Speed) dual mode; Supports ISP programming of devices with I2C, SPI, UART, BDM, MON, MW, JTAG, CAN, ICC, RS232 and any other serial port. ATE interface; Over-current and ESD protection to protect your equipment; DLL and API for easy integration into customers’ system.

## 3.JHD_162ALCD (16x2LCD)
This is 16 x 2 LCD Display with Yellow/Green Backlight ASCII Alphanumeric Character. 16×2 LCD Display Support mostly All Digital Microcontroller such as Arduino, 8051, PIC, AVR, ARM, MSP, COP8, STM, Raspberry Pi etc. About 16×2 LCD Display: 16×2 LCD is a basic 16 character by 2 line display Yellow/Green Back light.

## 4.1000uF capacitor
1000uF 25V Electrolytic Capacitor is a high quality electrolytic capacitor which offers long life and high reliability. Electrolytic Capacitors are most commonly used type of capacitors in Electronic Circuits. Electrolytic Capacitors have 2 Polars - Positive and Negative.

## 5. 10KΩ resistor (2 pieces)
Commonly used in breadboards and perf boards, these 10K resistors make excellent pull-ups, pull-downs, and current limiters.A 10k ohm resistor has 4 color band: brown, black, orange, and gold for 5% tolerance, respectively. To determine the value of a given resistor look for the gold or silver tolerance band and rotate the resistor as in the photo on the left.

## 6. HC-SR04 SENSOR
This is the HC-SR04 ultrasonic distance sensor. This economical sensor provides 2cm to 400cm of non-contact measurement functionality with a ranging accuracy that can reach up to 3mm. Each HC-SR04 module includes an ultrasonic transmitter, a receiver and a control circuit.There are only four pins that you need to worry about on the HC-SR04: VCC (Power), Trig (Trigger), Echo (Receive), and GND (Ground). You will find this sensor very easy to set up and use for your next range-finding project.This sensor has additional control circuitry that can prevent inconsistent "bouncy" data depending on the application. The HC-SR04 Ultrasonic Distance Sensor is a sensor used for detecting the distance to an object using sonar.The HC-SR04 uses non-contact ultrasound sonar to measure the distance to an object, and consists of two ultrasonic transmitters (basically speakers), a receiver, and a control circuit.
## Requirements :
## High Level Requirements
|ID|	DESCRIPTION|
|--|--|
|HLR01|Ultrasonic sensor should sense the echo.|
|HLR02|The LCD display must display the distance.|
|HLR03|The sensor must show the distance .|
|HLR03|The supply must turn on/off whrn switch is pressed.|


## Low Level Requirements
|ID|	Description	|
|--|--|
|LLR01|The 5V supply must turn on when the switch is pressed|	
|LLR02|The sensor must turn on when the switch is pressed.|	
|LLR03|The sensor must mesaure distance by echo within its specified range.|

## SWOT Analysis
![image](https://user-images.githubusercontent.com/98769359/157095785-c2eb5957-48ad-4477-a412-8eface854241.png)

## STRENGTHS
Easy to install, manage and maintain and low maintenance.
Highly reliable and Economically competitive.
## WEAKNESSES
The system may not show accurate distance after a certain distance range.
When a problem arose, there is no built-in function to help identify the source of the failure.
## OPPORTUNITIES
Distance can be used without using mesauring tapes or instruments.
## Threats
Skills for repair/spare parts not available in most of the areas.
Any sort of defect or fault in the circuit will cause problem in distance mesaurment.

## 4 W's and 1 H's
![4w and 1H](https://user-images.githubusercontent.com/98769359/157261225-a45eb048-ae29-4952-a0c0-73762bc70f5c.png)

## Who:
## o Everyone can use this device as for their commercial, industrial or domestic use.
## What:
## o This system is Automatic so it doesn't requires manual work which saves human time and energy.
## When:
## oThis system is used when the distance cannot be mesaured physically.
## Where:
## oIn places where mesauring distance physically is not possible.
## How:
## oThe ultrasonic sensor sends signals to the controller whenever it senses ECHO and display it on the LCD display .


## Block diagram

![Block diagram-1](https://user-images.githubusercontent.com/98769359/157241196-65f9d911-410c-400e-a646-04ffd13ed9d9.png)

## FlowChart
![Flowchart](https://user-images.githubusercontent.com/98769359/157241250-22a76733-572f-4195-93f7-1d6413ff85bd.png)

## TEST PLAN
## o For every feature,define a test case
## o How to run that feature
## o Define expected behaviour
## o Capture the actual result

## High Level Test Plan
|Test ID|Description|EXP I/P|EXP O/P|Result|
|--|--|--|--|--|
|HR_01|Turn on power supply|Power supply|Ultra-sonic sensor will turn ON/OFF|Passed|
|HR_02|Ultra-sonic should sense the ECHO or sound|There should be sound or a source of sound|Sensor will sense the sound|Passed|
|HR_03|LCD should display the distance|After sensing the micro controller will display the distance|Distance should be displayed|Passed|


## Low Level Test Plan
|Test ID|Description|Exp I/P|Exp O/P|Result|
|--|--|--|--|--|
|LR_01|Sensor should sense the sound when it is in a specified range|Sound in specified range|Sensor will sense the sound|Passed|
|LR_02|Sensor should not sense the sound when not in specified range|Sound is not in specified range|Sensor will not sense the sound|passed|
|LR_03|Distance should be displayed when sensor senses the sound|Taking input from controller|LCD will display distance |Passed|
|LR_04|Distance should not be displayed when sensor does not sese the sound|Taking input from the controller|LCD will not display distance|Passed|



## Codacy Badges
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/81c44f23f3004cd6ae702a98b3341a83)](https://www.codacy.com/gh/Shantanu3107/M2_EmbSys/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Shantanu3107/M2_EmbSys&amp;utm_campaign=Badge_Grade)

## Codiga badges
|Code Quality Score|Code grade|
|--|--|
|![image](https://user-images.githubusercontent.com/98769359/157088428-c379cbb3-d577-4cf1-9a81-f4d5051d4bb5.png)https://api.codiga.io/project/31636/score/svg |![image](https://user-images.githubusercontent.com/98769359/157088456-be5e6418-1f37-4e49-a4e1-980ecfaa0de0.png)https://api.codiga.io/project/31636/status/svg|



