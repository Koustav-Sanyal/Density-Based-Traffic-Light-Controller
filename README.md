# Density-Based-Traffic-Light-Controller
A  Smart Traffic Light Controller that ensures that signal of a particular direction should only function if there is traffic in that direction.


Components Required Density Based Traffic Light Controller Using Arduino
The components you are going to require for this project are as follows

1> Arduino Mega 2560

2> 4 X HC-SR04 ultrasonic sensors

3> 4 X Red LEDs

4> 4 X Green LEDs

5> 4 X Yellow LEDs

6> 12 X 220 ohm resistors

7> Jumper cables

Breadboards

The main purpose of this project is, if there will be no traffic on the other signal, one shouldn’t wait for that signal. The system will skip that signal and will move on the next one.


Arduino UNO is the main part of this project and it will be used to read from ultrasonic sensor HC-SR04 and calculate the distance. This distance will tell us if any vehicle is near the signal or not and according to that the traffic signals will be controlled.


 
 # The Circuit Diagram for this project is shown as:
 
 
 
   ![density_based_traffic_light_controller_bb_M2YCKtd7PL](https://user-images.githubusercontent.com/64331214/122291884-fa432f00-cf12-11eb-9a42-a8917302174b.png)



 #  Working of Density Based Traffic Light Controller Using Arduino:
 
The working of the project is divided into three steps:

1> If there is traffic at all the signals, then the system will work normally by controlling the signals one by one.

2> If there is no traffic near a signal, then the system will skip this signal and will move on to the next one. For example, if there is no vehicle at signal 2, 3 and currently the system is allowing vehicles at signal 1 to pass. Then after signal 1, the system will move on to signal 4 skipping signal 2 and 3.

3> If there is no traffic at all the 4 signals, system will stop at the current signal and will only move on the next signal if there will be traffic at any other signal.


                                                           
                                                           
