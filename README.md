# Course Reflection
Summarize the project and what problem it was solving.
-
This project was about building a state machine to represent low-level functionality of a thermostat. Using a Raspberry Pi 4 (RPi 4), peripheral equipment, and a Python script, the system sensed the air temperature and, depending on its current state, activated the heating or cooling mode until the air temperature reached the predetermined set point. The set point could be changed and modes could be cycled through via three buttons--one for set point increase, one for set point decrease, and one for state cycling.

What did you do particularly well?
-
I read through the existing code before writing any of my own. This taught me the inner workings of the program, like important variables, state transitions, and function interactions, which made completing TODO blocks easier. I also referenced the gpiozero library documentation for help with properly writing the fade in/fade out functionality for the LEDs. This showed me that using the blink() function made more sense than trying to change each LED's duty cycle, something done with a different GPIO library.

Where could you improve?
-
There were some mistakes I could've avoided with more careful proofreading before executing my code, like writing "processStateButton" instead of "processTempStateButton". I also needed refreshing on writing f strings in Python, a pretty foundational concept, which means I should be regularly practicing Python even if my courses don't always use it.


The function updateLights() was where I spent the most time developing and testing code. I sometimes ran into infinite loop situations by using while loops instead of if/elif statements. It might've saved me some trouble if I'd completed later TODO sections first, thus cementing the code's counter and altCounter in my mind before working on the pivotal updateLights().

What tools and/or resources are you adding to your support network?
-
With every programming project, I know that documentation is my friend. It was so easy to find the blink() function in the gpiozero documentation, and it was exactly what my project needed. Documentation and handy articles were also helpful for refreshers on f strings in Python. These kinds of resources are so valuable for my support network because they support the problem solving process.

What skills from this project will be particularly transferable to other projects and/or course work?
-


How did you make this project maintainable, readable, and adaptable?
-

