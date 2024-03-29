# Control Movement Using Deep Reinforcement Learning
Author: [Ng Zheng Jue](https://github.com/xinjue37), [Ng Rui Qi](https://github.com/Ruiqi2002)

* This is a project developed in undergraduate Year 2 - Semester 2
* This repository consists of **solving a control movement problem using Deep Reinforcement Learning**. The deep learning architecture used is CNN as we are dealing with the map. 
* One example of the environment map is at "[data_1.txt](https://github.com/xinjue37/Control-Movement-Using-Deep-Reinforcement-Learning/blob/main/data_1.txt)" where
  * The starting point is marked with 'S'
  * The obstacles are marked with 'W'
  * The passable route is marked with '.'
  * The targets are marked with 'T'.
* In the environment, the agent has a limited view at only 21x21* and the obstacle, 'W' will block the agent's view. The objective of this project is to design and implement a path-finding algorithm for a robot to find the optimal path from “S” to “T” and avoid the obstacles

* To formulate the problem as deep reinforcement learning problem, we need to define the state, action and reward:
  * State: 25x25 view from the current position where the extra view is filled by unknown if the agent haven't pass through that location
  * Action: The agent can move in 8 direction
  
|Index|Action|
|:-:|:-:|
|0|Right|
|1|Right Up|
|2|Up|
|3|Left Up|
|4|Left|
|5|Left Down|
|6|Down|
|7|Right Down|

  * Reward: if the agent reaches the target, add 10 rewards. However, the reward will keep decaying when time go by when the agent is does not reach the target.
* The detail explanation of the code can be found in the [Report.pdf](https://github.com/xinjue37/Control-Movement-Using-Deep-Reinforcement-Learning/blob/main/Report.pdf)
    
* This repository consists of
  - Jupyter Notebook file to extract the environment, process the environment, build the deep learning model, control movement using deep learning model
  - Sample map: 'data_1.txt'
  - 3 trained model 'CNN40000.pt', CNN50000.pt, CNN60000.pt
