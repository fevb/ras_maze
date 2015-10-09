RAS maze launch project
=======================

To start the simulated robot run:

```
roslaunch ras_maze_launch kobuki_maze.launch map_file:=/path_to_map/sample_map.txt publish_tf:=true
```

To drive the robot (using the arrow keys):

```
roslaunch kobuki_keyop keyop.launch
```

## Parameters

To start the robot from an arbitrary position, set the following parameters:

* x_offset
* y_offset
* theta_offset

Note that in rviz, the robot will be visualized correctly in the map frame (because the transform is set between the odom frame and the map frame). However, the robot position and orientation, as reported in the '/odom' topic will be set to 0 0 and 0 orientation when starting. Thus, if you're using this to simulate localizing from an unknown location, your task will be to compute the correct coordinates of the robot in the `/map` frame of reference.  

