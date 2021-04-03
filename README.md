# Ridgeback Examples

*Tested on **Ubuntu 18.04** with **ROS Melodic**.*

<img src="./doc/img/go_to_goal_full.gif" width="600">

Ridgeback examples provided by Ewha Glab. These examples depend on the [simulation](https://github.com/ridgeback/ridgeback_simulator), [visualization](https://github.com/ridgeback/ridgeback_desktop), [robot description and navigation](https://github.com/ridgeback/ridgeback) packages provided by Clearpath Robotics. 

You may use enviroments of your choice. The world used in the demo can be found under [./world](https://github.com/daeunSong/ridgeback_examples/world) and the map for this world can be found [./map](https://github.com/daeunSong/ridgeback_examples/map)

## Demo
Run the following commands in respective terminals.

set up before run:
```sh
roslaunch ridgeback_gazebo ridgeback_world.launch
```
for better performance, also run:
```sh
roslaunch ridgeback_navigation amcl_demo.launch
roslaunch ridgeback_viz view_robot.launch config:=localization
```

ridgeback example:
```sh
rosrun ridgeback_examples go_to_goal_full.py
```

