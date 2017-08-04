

For the Reverse Parking Experiment Only 

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
