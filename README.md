# Stride_assignment
## Commands for running
### 1.clone this repository into some folder.
### 2.open terminal and navigate to catkin_ws folder using "cd" command
### 3.u have to enter everytime u enter catkin_ws folder using new terminal
          '''    source ~/PATH_TO_FOLDER_U_STORED_CATKIN_WS/catkin_ws/devel/setup.bash  '''
    otherwise u can directly add this command to ~/.bashrc so that no need to enter it again and again
    echo "source ~/PATH_TO_FOLDER_U_STORED_CATKIN_WS/catkin_ws/devel/setup.bash" >> ~/.bashrc
### 4.now open 1st terminal and navigate to catkin_ws using cd commands(ros master runs)
     '''  cd catkin_ws
     catkin_make
     roscore  '''
### 5.similarily 2nd terminal(simulate gazebo with empty world)
     cd catkin_ws
     rosrun gazebo_ros gazebo
### 6.in 3rd terminal(spawn our robot into gazebo)
       cd catkin_ws
       roslaunch m2wr_description spawn.launch
then for controlling robot
    rosrun teleop_twist_keyboard teleop_twist_keyboard.py
now for controlling 
     pressing i moves forward
     pressing l rotates left
     pressing j rotates right
     pressing k stops robot.
     
