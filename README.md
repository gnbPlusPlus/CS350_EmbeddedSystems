# Course Reflection
Summarize the project and what problem it was solving.
-
This project was about building a state machine to represent low-level functionality of a thermostat. Using a Raspberry Pi 4 (RPi 4), peripheral equipment, and a Python script, the system sensed the air temperature and, depending on its current state, activated the heating or cooling mode until the air temperature reached the predetermined set point. 

Because this was a proof of concept and not a fully functional thermostat, no heating or cooling actually occurred, but instead the set point was altered to show that heating and cooling would start and stop as intended. The set point could be changed and modes could be cycled through via three buttons--one for set point increase, one for set point decrease, and one for state cycling.

What did you do particularly well?
-
I read through the existing code before writing any of my own. This taught me the inner workings of the program, like important variables, state transitions, and function interactions, which made completing TODO blocks easier. I also referenced the gpiozero library documentation for help with properly writing the fade in/fade out functionality for the LEDs. This showed me that using the blink() function made more sense than trying to change each LED's duty cycle, something done within a different GPIO library.

Where could you improve?
-
There were some mistakes I could've avoided with more careful proofreading before executing my code, like writing "processStateButton" instead of "processTempStateButton". I also needed refreshing on writing f strings in Python, a pretty foundational concept, which means I should be regularly practicing Python even if my courses don't always use it.


The function updateLights() was where I spent the most time developing and testing code. I sometimes ran into infinite loop situations by using while loops instead of if/elif statements. It might've saved me some trouble if I'd completed later TODO sections first, thus cementing the code's counter and altCounter logic in my mind before working on the pivotal updateLights().

What tools and/or resources are you adding to your support network?
-
With every programming project, I know that documentation is my friend. It was so easy to find the blink() function in the gpiozero documentation, and it was exactly what my project needed. Documentation and handy articles were also helpful for refreshers on f strings in Python. These kinds of resources are so valuable because they support the problem solving process.

What skills from this project will be particularly transferable to other projects and/or course work?
-
The work I completed for this course was all so new to me. I'd never worked with low-level electronic components of embedded systems before. I believe my experience from this project and other assignments will be directly transferrable to home and hobby projects, like building a custom display, but the conceptual knowledge is also part of what builds my strong foundation in computer science. As an aspiring UX designer, understanding the technical aspects of a physical product is a great advantage for communicating with developers and creating informed designs.

How did you make this project maintainable, readable, and adaptable?
-
I made this project maintainable, readable, and adaptable by keeping the comments consistent, using simple logic that made sense in context, and working in modularized sections. I also corrected any typos or unclear comments I encountered along the way. These actions combined make it so that any additional programmer picking up the code can read what's already there, understand the workflow, and add cohesive code as needed, using the functions and variables that already exist.
