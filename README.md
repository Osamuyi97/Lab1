University of Pennsylvania, ESE 5190: Intro to Embedded Systems, Lab 1


Osamuyi Uwadia
 
 https://www.linkedin.com/in/osamuyi-uwadia-a3038813b/

Tested on : HP Spectre x360 Convertible 15-df1xxx Microsoft Windows 11



General Information 

In Q3.2 for the Firefly Program, the Embedded System (RP2040) will use the RGB LED to tracks the brightness reading from the color sensor (APDS9960). We want the senor to be able to determine if pointed at something bright the RGB LED would light up and if covered up the RGB LED is dim down  
In Q4.4 for the Custom Real Time Visualizer, we can use the sensor (APDS9960) as a keyboard in order in produce Real Time values that is the same as typing on a word document but instead of using a “keyboard” we use a sensor.


Walkthrough

Firefly
•	The Firefly program use the RP2040 and the APDS9960
•	The RP2040 use the neopixel to change the RGB color values 
•	The code will put a limit in on brightness and dim values. 
•	At a certain value the RGB will turn on but if that value where to fall back down the brightness will decrease instantly 
•	The color_integration_time helps increase the response time between two sensor values  

https://github.com/Osamuyi97/Lab-1/blob/main/20220930_200545_1.gif

Keyboard Emulator - Q4.4
•	The RP2040 will be used as a keyboard in this Program
•	RP2040 will be used and given parameters to sense the brightness. 
•	Depending on the level read by the RP2040 it will:
o	Write continuous O’s
o	Continuous Backspace (Erase)  
o	Do Nothing  

•	They are also shown by a RGB LED
o	Continuous O’s: PURPLE 
o	Continuous Backspace: RED
o	Do Nothing: Clear 
•	Have a (Do Nothing) setting is the bread and butter of this Program because it allows RP2040 not to go on an endless loop of O’s and Backspace.
•	Very Usefully when your program wants to go erase everything including your code!!


https://github.com/Osamuyi97/Lab-1/blob/main/20220930_195752_1.gif 

https://github.com/Osamuyi97/Lab-1/blob/main/20220930_195849_2.gif

https://github.com/Osamuyi97/Lab-1/blob/main/20220930_195942_1.gif


A Simple Flowchart

https://github.com/Osamuyi97/Lab-1/blob/main/Adafruit.docx
