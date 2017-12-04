## to start run this commands


$ sudo apt-get update

$ sudo apt-get install python-catkin-tools

$ cd catkin_ws

$ source ~/catkin_ws/devel/setup.bash

$ source ~/.bashrc

**to launch the robot in gazebo:**

$ roslaunch mybot_gazebo mybot_world.launch

**to move the robot**

$ rostopic pub /cmd_vel geometry_msgs/Twist "linear 

**press the tab key after the last command then make the changes before pressing enter
it should look like this:**

rostopic pub /cmd_vel geometry_msgs/Twist "linear:
  x: 0.5
  y: 0.0
  z: 0.0
angular:
  x: 0.0
  y: 0.0
  z: 0.2"

**after you make the changes press enter and the robot should start moving on Gazebo**


**this would launch the robot in RVIS**

$ roslaunch mybot_description mybot_rviz.launch







