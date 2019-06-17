# multi_map_server

put this in ~/catkin_ws/src/

If you do this correctly, you will only have to pull from here once.

1. Make sure the multi_map_server is in the correct part of the tree.
2. Go to /opt/ros/kinetic/share/turtlebot_navigation/launch and find the amcl_demo.launch file
3. Replace the contents of the launch file with the amcl_demo.launch file provided in this repository
4. Pull from the robot_summer repository if you haven't already
5. Do a catkin_make in the catkin_ws
6. IF YOU ARE WORKING IN SIMULATION, leave the service client within teleport_node of ~/robot_summer/src untouched. The client will not be able to work in simulation due to the nature of Stage. However you should be able to search and call for the service in the terminal (It will do nothing) or run it if you like.
7. IF YOU ARE WORKING IN HARDWARE, uncomment the service client. Fix the paths to the files if necessary
