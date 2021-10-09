# udm_dave_gb
This repo contains Part 1 &amp; Part 2 of CFDL labs in MIAR on using a Turtlebot3 WafflePi for mapping and navigation.

## Step 1
### Ensure the following packages are installed. Note that not all of them are required.
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/ROBOTIS-GIT/turtlebot3.git
$ git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git
$ git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
$ git clone https://github.com/ROBOTIS-GIT/turtlebot3_applications.git
$ git clone https://github.com/ROBOTIS-GIT/turtlebot3_applications_msgs.git
$ cd .. && catkin_make
$ source devel/setup.bash
```
## Step 2
### Download and install the git repo.
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/azezezaaa/udm_dave_gb.git
$ cd ~/catkin_ws/
$ catkin_make && source devel/setup.bash
```
## Step 3
### Terminal A
```
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch
```
### Terminal B
```
$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch
```
### Terminal C
```
$ rosrun udm_dave_gb global_localization.py
```





