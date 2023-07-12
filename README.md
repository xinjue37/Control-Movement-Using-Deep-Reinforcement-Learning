# Undergraduate-Y2S2-Control_Movement_Using_Deep_Reinforcement_Learning
Author: Ng Zheng Jue, Ng Rui Qi

* This is a project developed in undergraduate Year 2 - Semester 2
* This repository consists of solving a control movement problem using Deep Reinforcement Learning. The deep learning architecture used is CNN as we are dealing with the map
* This repository consists of
  - Jupyter Notebook file to extract the environment, process the environment, build the deep learning model, control movement using deep learning model
  - Sample map: 'data_1.txt'
  - 3 trained model 'CNN40000.pt', CNN50000.pt, CNN60000.pt

## Environment
Given “data_1.txt” as one of a sample map, where the starting point is marked with 'S', the obstacles are marked with 'W', the passable route is marked with '.', and the targets are marked with 'T'. *The agent has a limited view at only 21x21*.

## Objective 
Design and implement a path-finding algorithm for a robot to find the optimal path from “S” to “T” and avoid the obstacles
