# Ultrasound-robot

WOKWI Project link: https://wokwi.com/projects/403081427638509569 

simulating a robot that uses ultrasound sensor that control its servo motors.
the idae of this project is to simulate a robot that uses an ultrasound sensor to determine if it should walk or stop.
first i connected an LED light to get familiar with the esp32 board.
then i connected the ultrasound sensor to the esp.
the echo pin needed to be connected to an input port.
but the trig pin needed to be connected to an output port, which gave me a long time to figure out. 
(because i was connecting it to an input only port and the whole code was not working)
the servo motors were connected without trouple as i was familiar with them from the previous project.

in the code set up i attached all the devices to their respective ports.
i made the LED light keep blinking to test the esp32 board.

then i made the ultrasound sensor trig pin send out a sonic burst.
using the echo pin we can sense the sonic burst coming back.
from the echo pin input i use a code to calculate the distance.

if the distance is greater than 100m i make the servo motors move like they are robot legs.
if the distance is less than 100m, the legs stop moving (simulating getting close to a wall or an object).
