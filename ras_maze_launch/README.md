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

* `publish_tf` : true/false - whether to publish a static transform between the robot `/odom` frame and the map `/map` frame. 
