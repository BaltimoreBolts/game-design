# game-design
python/cad game design micro meet

# Skills
- linux (command line)
- git
- python
- cad

# Ideation
- maze
- sensors/cameras
- autonomous vs user control

# Terminology
- ROS : Stanford's Robot Operating System
- CLI : Command Line Interface (Terminal)
- Catkin : ROS's build system
- Gazebo : Simulated reality viewer
- RViz : Robot's sensors and perspective data

# Commands
### Building
- `catkin_make`
- `source devel/setup.sh`
- `export TURTLEBOT3_MODEL=burger`

### Running
- Launch the Gazebo world to visualize the robot and its environment
    `roslaunch turtlebot3_gazebo turtlebot3_house.launch`
- Control the robot using your keyboard
    `roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch`
- Have the robot autonomously drive itself
    `roslaunch turtlebot3_gazebo turtlebot3_simulation.launch`
- Have the robot map its world
    `roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping`
