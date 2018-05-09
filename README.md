# Electromagnetic_Compass_Final_Version
My 387 Final Project

# Periferals:
* -Xilinx PYNQ Board with PMOD Grove Adapter and Shield
* -Grove IMU 9DOF v2.0
* -Grove OLED
* -Potentiometer

# Overview:
The goal of this project Is to create an programable electronic compass that will always point at the desired 
Lattitde/Longitude coordinates. This is done by using the Xilinx PYNQ Board to control the Grove IMU 9DOF v2.0
chip and webscraping freegeoip.net to find the current board's current location based on IP address. The current location of the compass,
target coordinates, and desired direction are then conveyed to the user Via the OLED.

# Current State:
As of 5/8/18 the compass will webscrape of the current location and magnetic declination associated with that location, and use these
pieces of data to calculate the bearing from north to that target coordinates. This is then compared to the compass value which is used
create the bearing between the direction the compass is pointed and he target. All of this data is then displayed on th OLED for the user,
and is constantlu updated in real time, refreshing roughly every second.

<img src="https://github.com/NickyNocerino/Electromagnetic_Compass_Final_Version/blob/master/20180508_232018.jpg" width="400">
