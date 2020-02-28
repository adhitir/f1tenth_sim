
#Gazebo Model and Environment for F1Tenth 

This project is developed in and tested on ROS Indigo. Created primarily to procure datasets for a machine learning model on reverse parking. 


The results of that project can be found in this paper:
Li, Rui, Wang, Weitian, Chen, Yi, Srinivasan, Srivatsan, and Krovi, Venkat N. "An End-to-End Fully Automatic Bay Parking Approach for Autonomous Vehicles." Proceedings of the ASME 2018 Dynamic Systems and Control Conference. 

First terminal:

cd /f1tenth_sim
. devel/setup.bash
roslaunch f1tenth_gazebo f1tenth_reverse_parking.launch 

Second terminal:
cd /f1tenth_sim
. devel/setup.bash
roslaunch f1tenth_control record_rosbag.launch 


Third terminal:
cd /f1tenth_sim
. devel/setup.bash
rosrun f1tenth_control bag_to_images.py [trial number]
