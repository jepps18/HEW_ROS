# Homeostasis Enabling Wheel Model - General Notes

## How to begin
1) Create a catkin workspace on your local computer  
	$ mkdir -p ~/catkin_ws/src  
	$ cd ~/catkin_ws/  
	$ catkin_make  
	
2) Clone the repository $ git clone https://github.com/jepps18/HEW_ros.git  
	$ cd ~/catkin_ws/src  
	$ git clone https://github.com/jepps18/HEW_ROS.git  
3) Build the catkin workspace  
	$ cd ~/catkin_ws  
	$ catkin_make  
	$ source devel/setup.bash  

## How to launch the HEW Model  
	$ cd ~/catkin_ws  
	$ roslaunch any_name hew_world.launch   

## How to move a joint (Example Arm)  
In a terminal run the following command  
	$ rostopic pub -1 /hew/joint1_positon_controller/command std_msgs/Float64 "data: 0.7".  
The ros topic for the large arm is /hew/joint1_position_controller/command   
The ros topic for the horizontal transmssion (the part that drives the wheel) is /hew/joint2_position_controller/command   

Notes:  
-The currenet model may not look like the actual vehicle yet. The vehicle is being imported via an iterative process.  
-Everytime catkin_make is used you must source devel/setup.bash  

## Useful Resources  
-http://wiki.ros.org/ros_control  
-The PID values in the hew_control.yaml file need to be adjusted, damping value in URDF file also needs adjusting
