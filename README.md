# MoveIt integration for Poppy Ergo Jr in ROS 1

![Poppy Ergo Jr in RViz ROS Melodic](https://raw.githubusercontent.com/poppy-project/poppy_ergo_jr_description/master/doc/img/rviz.png)

This package is meant to be used with the following packages:
* [Poppy controllers](https://github.com/poppy-project/poppy_controllers#ros-melodic-controller-for-poppy-robots) that run on the robot
* [Poppy Ergo Jr description (URDF)](https://github.com/poppy-project/poppy_ergo_jr_description)

This package has been tested with Melodic and Noetic.

## Quickstart
### With a simulated robot
Start MoveIt in simulation if you have assembled your robot with the gripper effector:
```bash
roslaunch poppy_ergo_jr_moveit_config demo.launch fake_execution:=true gripper:=true
```
...if you have assembled your robot with the lamp effector:
```
roslaunch poppy_ergo_jr_moveit_config demo.launch fake_execution:=true lamp:=true
```

### With a real robot
Make sure the Poppy Controllers are running on your robot and then just set `fake_execution` to `false`:
```
roslaunch poppy_ergo_jr_moveit_config demo.launch fake_execution:=false lamp:=true
```
