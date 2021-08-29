# Another_ROS_robot_with_SLAM
**This Repository will explain the 3rd Task 
## Requirements:
- Use another ROS robot to creat and save a map.
## Steps:
1. Using this package to provide a simulation environment of a warehouse. A robot is simulated at the center of the environment, with 2D laser scanner provided. 
2. Install ROS package `sudo apt-get install ros-melodic-hector-trajectory-server ros-melodic-slam-gmapping ros-melodic-navigation
`
3. Then
- `cd ~/catkin_ws/src`
- `git clone https://github.com/faisalsaud63192/warehouse_simulation_toolkit`
- `cd ..`
- `catkin_make`
- `source ~/catkin_ws/devel/setup.bash`
4. Launch ROS
 - `roslaunch warehouse_simulation warehouse_simulation.launch`
 
 -
 ![gazebo](https://github.com/faisalsaud63192/Another_ROS_robot_with_SLAM/blob/main/gazebo.png)
 
 ![rviz](https://github.com/faisalsaud63192/Another_ROS_robot_with_SLAM/blob/main/rviz.png)
 
 5. Autonomous Navigation by setting a target points in RVIZ and the robot will navigate to the location in gazebo. 
   - click 2d nav goal button on rviz and then click any points you want on the map.
   
   ![rviz2](https://github.com/faisalsaud63192/Another_ROS_robot_with_SLAM/blob/main/rviz2.png)
   
   ![gazebo2](https://github.com/faisalsaud63192/Another_ROS_robot_with_SLAM/blob/main/gazebo2.png)
   
 6. When the map is created successfully in Rviz, open new terminal and save it using the command `rosrun map_server map_saver -f ~/map`
 
 ![terminal](https://github.com/faisalsaud63192/Another_ROS_robot_with_SLAM/blob/main/terminal.png)
 
 ![map-image](https://github.com/faisalsaud63192/Another_ROS_robot_with_SLAM/blob/main/map_image.png)
 
 - simulation video in video_simulation.webm file
 - saving map in map.pgm
 
 7. Task is done.
