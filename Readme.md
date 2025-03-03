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
