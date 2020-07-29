# Build-My-World

Project 1 of Udacity Robotics Software Engineering Nanodegree Program 

## Overview of the project

In this project I haved created a simulation world in Gazebo for all the upcoming projects in the Udacity Robotics Software Engineer Nanodegree Program.

The tasks for this project were:
1) Build a single floor wall structure using the Building Editor tool in Gazebo. Apply at least one feature, one color, and optionally one texture to your structure. Make sure there's enough space between the walls for a robot to navigate.
2) Model any object of your choice using the Model Editor tool in Gazebo. Your model links should be connected with joints.
3) Import your structure and two instances of your model inside an empty Gazebo World.
4) Import at least one model from the Gazebo online library and implement it in your existing Gazebo world.
5) Write a C++ World Plugin to interact with your world. Your code should display “Welcome to <your name>’s World!” message as soon as you launch the Gazebo world file.

## What you will need to run 
* Gazebo >= 7.0
* ROS Kinetic
* make >= 4.1 (Linux. make is installed by default on most Linux distros )

## Project Description
Directory Structure 
* Udacityoffice.world: Gazebo world file 
* floor: Floor structure built bu Building Editor of Gazebo 
* robot: A robot built by Model Editor of Gazebo 
* welcome.cpp: Gazebo world plugin C++ script 
* CMakeLists.txt: File to link the C++ code to libraries 

## How to run 
* Clone this repository
* Create a build directory 
* In the build directory, compile your code with
cmake .. 
* Followed by 
make 
* Export your plugin folder in the terminal so your world file can find it :
export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/P1-Build-My-World/build
* Launch the world file in Gazebo to load both the world and plugin 
cd /home/workspace/P1-Build-My-World/world/
gazebo Udacityoffice.world

