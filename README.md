# Density-Based-Traffic-Light-Controller
A  Smart Traffic Light Controller that ensures that signal of a particular direction should only function if there is traffic in that direction.


                 Components Required for Density Based Traffic Light Controller Using Arduino Mega

The components you are going to require for this project are as follows:

1> Arduino Mega 2560

2> 4 X HC-SR04 ultrasonic sensors

3> 4 X Red LEDs

4> 4 X Green LEDs

5> 4 X Yellow LEDs

6> 12 X 220 ohm resistors

7> Jumper cables

8> Breadboards


The main purpose of this project is to ensure that if there will be no traffic on one signal, one shouldn’t wait for that signal. The system will skip that signal and will move on the next one.


Arduino Mega is the main part of this project and it is used to read the time from the ultrasonic sensor HC-SR04 and calculate the distance of the object from the signal. This distance will tell us if any vehicle is near to the signal (Under 5cm distance here) or not and according to that the traffic signals will be controlled.


 
 # The Circuit Diagram for this project is shown as:
 
 
 
   ![density_based_traffic_light_controller](https://user-images.githubusercontent.com/64331214/146633463-d9f67cd6-1a04-420e-998c-51c8dfb5f11b.png)




 #  Working of Density Based Traffic Light Controller Using Arduino:
 
The working of the project is divided into three steps:

1> If there is traffic at all the signals, then the system will work normally by controlling the signals one by one.

2> If there is no traffic near a signal, then the system will skip this signal and will move on to the next one. For example, if there is no vehicle at signal 2, 3 and currently the system is allowing vehicles at signal 1 to pass. Then after signal 1, the system will move on to signal 4 skipping signal 2 and 3.

3> If there is no traffic at all the 4 signals, system will stop at the current signal and will only move on the next signal if there will be traffic at any other signal.

4> The traffic at a signal is found by considering whether any object is present within 5cm distance from the ultrasonic sensor. The distance is determined by emitting ultrasonic waves from the HC-SR04 ultrasonic sensors, and calculating the time after which the echo is received if the waves reflect back after striking any nearby object. Then the distance of the object from the sensor is calculated by the formula: (Distance = Speed of wave * Time taken to hear the echo/2). 

If the distance comes to be greater than 5cm, then the LEDs do not operate, or else they come under operation.


                                                           
                                                           
