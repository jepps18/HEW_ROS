# Homeostasis Enabling Wheel Model - General Notes

## How to begin
1) Create a catkin workspace on your local computer  
	$ mkdir -p ~/catkin_ws/src  
	$ cd ~/catkin_ws/  
	$ catkin_make  
	
3) Clone the repository $ git clone https://github.com/jepps18/HEW_ros.git  
	$ cd ~/catkin_ws/src  
	$ git clone https://github.com/jepps18/HEW_ROS.git  
4) Build the catkin workspace  
	$ cd ~/catkin_ws  
	$ catkin_make  
	$ source devel/setup.bash  

## How to launch the HEW Model  
	$ cd ~/catkin_ws  
	$ roslaunch any_name hew_world.launch  

Note: The currenet model may not look like the actual vehicle yet. The vehicle is being imported via an iterative process. 