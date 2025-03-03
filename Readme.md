# Wokwi Project Link: -
https://wokwi.com/projects/423474162534233089

# Task-1:- Blow on the sensor and observe whether it detects minor changes in temperature and humidity.
Yes, It changes the temperature and humidity after a warm blow on the sensor. My Humidity changes from 50% to 54% and Temperatures rises from 23C to 25C.

# Task-2:- Running the Code Without Interrupt

        With Interrupts:-
1- When the button is pressed it is detected.
2- The CPU was free to perform other tasks without checking the button constantly.
3- Allowing other tasks to perform their execution without blocking them.

        Without Interrupts:-
1- The button press is checked once per loop iteration, leading to delays.
2- The system continuously checks for a button press i.e (Polling).
3- CPU spent more time in checking the state of button leading other exections of program in delay.

# Task-3:- Understanding debouncing issue
1. What is a Debounce Issue and Why Do We Get Rid of It?
A debounce issue occurs when a button or switch is pressed, and instead of registering a single action, it generates multiple signals due to mechanical or electrical noise. This is common in mechanical switches, keypads, and hardware sensors, where physical contacts bounce before settling into a stable state.
1. Multiple unintended inputs
2. Inaccurate sensor readings
3. Glitches in user experience

2. Applications Where Debounce Issues Can Be Critical
Debounce issues can be critical in applications where precise and reliable inputs are required. Here are some key areas where debouncing is essential:
1. Embedded Systems & IoT Devices
2. Consumer Electronics
3. Automotive Systems
4. Medical Devices
5. Robotics & Automation

3. Why Does Debounce Occur?
When a mechanical switch or button is pressed or released, the contacts inside do not instantly settle into their final state. Instead, they bounce between ON and OFF multiple times within a few milliseconds before stabilizing. This bouncing can cause unintended multiple detections instead of a single press.

# Is debounce a compiler error?
No. A compiler error occurs due to syntax mistakes in the code. Debounce is a hardware issue, not related to the compiler.

# Is debounce a logical error?
No. A logical error happens when a program runs but produces incorrect results due to mistakes in logic. Debounce is an electrical/mechanical issue, not a programming logic mistake.

# Does debounce happen because the microcontroller is cheap?
Not necessarily. Even high-end microcontrollers will experience debounce if they process raw switch input without any filtering. The issue is in the mechanical switch, not the microcontroller.

# How to fix debounce?
Debouncing can be handled using:
1. Hardware solutions – Adding a capacitor (RC circuit) or using Schmitt trigger circuits.
2. Software solutions – Implementing a debounce delay in code using timers or software filters.