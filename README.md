# PolicyGrid

Course: COMP 4766 Introduction to Autonomous Robotics

Topics: Reinforcement learning, policy iteration, policy evaluation, dynamic programming

Professor: Dr. Andrew Vardy https://www.mun.ca/engineering/about/our-people/andrew-vardy/

Additional resources: https://towardsdatascience.com/reinforcement-learning-101-e24b50e1d292

A special thanks to Dr.Andrew Vardy for a great semester and also for giving me permission to post this assignment. Unfortunately, I am unable to post the Python file as it will be a violation against MUN's academic integrity. If you have any questions please contact me at klan@mun.ca. All credits to Dr.Vardy for designing the assignment structure. 

Assignment set up: The set of possible actions from all states is {up, down, right} (left is not available).  While these actions are available in all states, they do not always affect the robot's state.  For example, in state d the "right" action can be executed but the robot will remain in state d.  The situation is similar at the borders, for example in state f executing "down" leaves the robot in state f.  Our model of this system is deterministic.  This means that the probabilities for all state transitions are either 0 or 1.

Executing any action in state c will result in a reward of +10.  Executing any action in any other state gives a reward of 0.

![Screen Shot 2022-12-14 at 1 11 51 PM](https://user-images.githubusercontent.com/66441548/207655431-048c7645-b120-473f-8589-e10aab77d796.png)


Self.occupancy: represents in the grid is occupied (1 presents the red blocks that are not available)

self.policy_y_array: represents the movement along the y axis (up and down)

self.policy_x_array: represents the movement along the x axis (right)

self.reward: represents the rewards that each grid has (in this case only state C)

![Screen Shot 2022-12-12 at 4 41 38 PM](https://user-images.githubusercontent.com/66441548/207653100-99e394fe-f0c2-414c-9a38-2f7bc09a0032.png)

For this assignment, the students were required to hand calculated three iterations of policy evaulation and one iteration of policy improvement. Then using the results as a guide, students must implement Dynamic Programming (DP) for the grid world using Python. The students must also have to figure out how make the algorithm converge and present the path that will result in the biggest reward (which is being in state C and excuting from there) 

![Screen Shot 2022-12-12 at 4 41 21 PM](https://user-images.githubusercontent.com/66441548/207652586-57901b02-e14a-4589-b77e-1c441eff2cba.png)
