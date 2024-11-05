# Brake-Actuators

Brake Actuator Logic:
1. Listen for OK signal on CANBUS
2. Listen for BRAKE COMMAND from operator
3. If OK signal is lost
4. If BRAKE COMMAND is high
5. Actuate brakes
6. Else
7. Else
8. Keep listening

Perhaps using a while loop is better? 

What we have to do is: 
braking.cpp: set power signal of brake actuator to HIGH for certain number of seconds 
listen.cpp: listen for CANBUS commands, then call functions from BRAKE.CPP 
