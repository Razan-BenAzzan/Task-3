# Task-3
task 3

downloading smart method's robotic arm joint stick package in ROS and working on it


after downloading ROS on your virtual box

- open "Terminal" 
- make a catin workspace by using these commands:
   mkdir -p ~/catkin_ws/src

   cd ~/catkin_ws/

   catkin_make

   cd ~/catkin_ws/src

 - accessing arm packages  commands: https://github.com/smart-methods/arduino_robot_arm 
    cd ~/catkin_ws

    rosdep install --from-paths src --ignore-src -r -y
    $ sudo apt-get install ros-noetic-moveit

    $ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui

    $ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher

    $ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
- add the workspace in the bashrc file using the following command 
   sudo nano ~/.bashrc
   source /home/YourVirtualName/catkin_ws/devel/setup.bash [change YourVirtualName to your own name]
- save it and exit
-  to launch RVIZ program to work on the robotic arm :
     source ~/.bashrc

     roslaunch robot_pkg check_motors.launch

 
