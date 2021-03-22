# Ridgeback

*Tested on **Ubuntu 18.04** with **ROS Melodic**.*

<img src="./doc/img/go_to_goal_full.gif" width="600">

## Build and Compile

1. Clone this repository:
  ```sh
  cd your/catkin_ws
  cd src
  git clone https://github.com/daeunSong/ridgeback_examples
  ```

2. Install the dependencies:
  ```sh
  git clone https://github.com/ros-teleop/teleop_twist_keyboard
  cd .. 
  cd catkin_make
  ```

3. Source the workspace:
  ```sh
  source ~/.bashrc
  ```

4. Extra files:
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

