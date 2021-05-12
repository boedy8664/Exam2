# Exam2
## About the project:
This project is about using mbed to run a RPC loop with a custom functions (operation modes): (1) gesture UI, and feature the gesture by
tilt angle detection
## Built with:
C++, Python
## Equipment
1. PC
2. B_L4S5I_IOT01A
3. uLCD display
## Description
mbed run the RPC loop to get input string commands from PC/Python, and it will in turn call custom RPC functions.
The purpose of the features is to differentiate accelerator data 
by their classified gesture, e.g., circle vs. z-shape. They are manually tuned features for classification.
After the PC/Python gets a preset number of gesture events, e.g., 10, from the broker, it sends a command to mbed to stop
the accelerator capture mode. Therefore, the mbed is back to RPC loop.
After the PC/Python send the stop command, please send another command to retrieve the saved feature data.
