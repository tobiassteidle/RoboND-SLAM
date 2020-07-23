[![Udacity - Robotics NanoDegree Program](https://s3-us-west-1.amazonaws.com/udacity-robotics/Extra+Images/RoboND_flag.png)](https://www.udacity.com/robotics)

# RoboND_SLAM
Robotics Software Engineer Project "Where Am I"

### Used Packages
[gmapping](http://wiki.ros.org/gmapping)

### Steps to launch the simulation

#### Step 1 Update and upgrade the Workspace image
```sh
$ sudo apt-get update
$ sudo apt-get upgrade -y
```

#### Step 2 Install dependencies
```sh
$ cd ..
$ source devel/setup.bash
$ rosdep -i install turtlebot_gazebo
$ rosdep -i install turtlebot_teleop
```
#### Step 3 Compile the code
```sh
$ catkin_make
```

#### Step 4 Source ROS in this workspace
```sh
$ source devel/setup.bash
```

#### Step 5 Run the Simulation  
```sh
$ roslaunch my_robot world.launch
```

#### Step 6 Navigate trought environment
```sh
$ roslaunch turtlebot_teleop keyboard_teleop.launch
```

#### Step 7 Save Map  
With the map_server you can load and save maps. Running map_server will generate the map.pgm and the map.yaml files.
```sh
$ rosrun map_server map_saver -f myMap
```

### Output
![alt text](images/output_1.png)
![alt text](images/output_2.png)


