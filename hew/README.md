# Homeostasis Enabling Wheel Model - General Notes

## How to begin
1) Create a catkin workspace on your local computer  
	$ mkdir -p ~/catkin_ws/src  
	$ cd ~/catkin_ws/  
	$ catkin_make  
2) Create a catkin package (You can name it anything you'd like just replace "any_name" with the name you'd like.)
	$ cd ~/catkin_ws/src  
	$ catkin_create_pkg any_name std_msgs rospy roscpp  
3) Clone the repository $ git clone https://github.com/jepps18/HEW_ros.git  
	$ git clone https://github.com/jepps18/HEW_ROS.git  
4) Build the catkin workspace  
	$ cd ~/catkin_ws  
	$ catkin_make  
	$ source devel/setup.bash  

## How to launch the HEW Model  
	$ cd ~/catkin_ws  
	$ roslaunch any_name hew_world.launch  

Note: The currenet model may not look like the actual vehicle yet. The vehicle is being imported via an iterative process. 