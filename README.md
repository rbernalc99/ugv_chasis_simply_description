# ugv_chasis_simply_description
UGV simplified model. The dynamics of the track are neglected considering a basic operation of the robot, modelled has a skid steer drive. 

To run the model description. Add the library to the ~/catkin_ws/src directory. 
Change directory to  ~/catkin_ws
Run catkin_make command

To run rviz run the following command on the terminal: roslaunch ugv_chasis_simply_description display.launch
To run gazebo run the following command on the terminal: roslaunch ugv_chasis_simply_description gazebo.launch

In order to simulate the skid steer drive I used the gazebo plugin available in: https://classic.gazebosim.org/tutorials?tut=ros_gzplugins

Run "rostopic list" to check that the topic /cmd_vel is available. This topic message is of the geometry_msgs/Twist 
I used the teleop_twist_keyboard package which controls the Twist via keyboard.
Previous to running the teleop_twist_keyboard script, initialize the simulation time on gazebo.


![default_gzclient_camera(1)-2022-07-12T10_41_19 487163](https://user-images.githubusercontent.com/107320063/178533167-fd67b58f-0857-47e1-b6b9-413ad6dee6a7.jpg)
