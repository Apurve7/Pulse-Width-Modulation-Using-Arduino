# Pulse-Width-Modulation-Using-Arduino

This project demonstrates how to control the brightness of an LED using Pulse Width Modulation (PWM) with an Arduino. The code slowly increases the LED's brightness in discrete steps over a long period.

Functionality ⚙
This program uses the analogWrite() function to control an LED connected to a PWM-capable pin on the Arduino.

Pulse Width Modulation (PWM): Instead of just being ON or OFF, PWM allows the Arduino to simulate an analog voltage. It does this by rapidly switching the pin on and off. The "duty cycle" is the percentage of time the pin is ON. A low duty cycle (e.g., 10%) makes the LED appear dim, while a high duty cycle (e.g., 90%) makes it bright.

Code Behavior: The code starts with a duty_cycle_value of 1 (very dim). It sets the LED to this brightness and then waits for 3 seconds (delay(3000)). After the delay, it increments the duty_cycle_value by one and repeats the process.

The LED will get noticeably brighter every 3 seconds, stepping through all 254 levels of brightness. This gradual increase will take approximately 12.7 minutes to complete (254 steps × 3 seconds/step). Once it reaches the maximum brightness, it will remain at that level.

Hardware Requirements 🔩
Arduino Uno (or any compatible board)

1 x LED (any color)

1 x 220Ω Resistor

Breadboard

Jumper Wires

Software Requirements 💻
Arduino IDE

Circuit and Connections 🔌
You must connect the LED to a PWM pin on the Arduino, indicated by a tilde symbol (~). The code specifies pin 9.

Connect the long leg (anode) of the LED to one end of the 220Ω resistor.

Connect the other end of the resistor to Arduino Pin 9.

Connect the short leg (cathode) of the LED to the Arduino GND pin.

How to Use 
Assemble the circuit as described above.

Connect your Arduino to your computer via USB.

Open the Arduino IDE and paste the provided code into a new sketch.

Upload the sketch to your Arduino board.

Observe the LED. It will start very dim and slowly get brighter in noticeable steps every 3 seconds.












Tools

