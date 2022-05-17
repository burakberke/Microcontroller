# Microcontroller
The purpose of the project is to control the position of a DC motor with inputs given from the 
user via the PIC microcontroller.The inputs are a reference angle and the proportional gain 
parameter Kp.Also, the controller does not execute another code and process until the input 
value Kp is received. Reference angle of the second input is obtained from an analog voltage 
divider reading.It is converted using the ADC converter module of the microcontroller. 
Another input then used to calculate the reference angle and instantaneous position is based 
on the motor encoder input.The position error is calculated and the starting position of the 
motor is always 0 degrees. Finally, the shorter direction to be turned is calculated. After all 
calculations and readings.We output a pwm signal to the motor enable pin to set its speed 
with a certain duty cycle based on a function of Kp and error. We set the motor driver's input 
pins to high or low according to the shorter turning direction calculated.When there are no 
more errors, the motor has reached the desired position and the motor is stopped.
