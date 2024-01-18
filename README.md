# NIOSR-Project

Projekt zaliczeniowy z Niosr 

Wymagania:

instalacja ros2:

https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html

instalacja turtlebot3 package:

sudo apt install ros-humble-turtlebot3*



Uruchomienie paczki:

Terminal 1:


cd ~/ros2_ws

source install/setup.bash

ros2 run camera_subscriber camera_node

Terminal 2:


cd ~/ros2_ws

source install/setup.bash

export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:ros2 pkg \ prefix turtlebot3_gazebo \ /share/turtlebot3_gazebo/models/

ros2 launch turtlebot3_gazebo empty_world.launch.py
