# dual_robotiq

This repository provides our customized ros package for simultaneous use of two robotiq 3F gripper.        


## Features
- Simulation and execution of two robotiq 3F addaptive gripper simultaneously
- Mode: basic, pinch, wide scissor
- Action: close, open

## Usage
### Simulation
Currently, simulation can only run in a [dual_ur_robotiq](https://github.com/yaesolKim/dual_ur_robotiq) library integrated with UR5e.

### Actual gripper execution: Bring up grippers and robots, Run moveit and Rviz   
Run the lines below in the respective terminals.
```commandline
roscore
roslaunch robotiq_3f_gripper_control dual_gripper_tcp.launch
roslaunch robotiq_3f_gripper_joint_state_publisher dual_gripper_joint_state_publisher.launch
roslaunch robotiq_3f_gripper_visualization robotiq_gripper_upload.launch
```

<!--
```commandline
rosrun robotiq_3f_gripper_control Robotiq3FGripperSimpleController.py  
rosrun robotiq_3f_gripper_control Robotiq3FGripperStatusListener.py
```
-->
