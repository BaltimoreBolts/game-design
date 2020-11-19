# Game Design
Python/CAD/ROS Game Design Micro Meet

# Information
The game design goal is to create a game using real-world, virtual, or hybrid design elements, and compete for judged awards. Winning concepts will be considered for use in future official games. 

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

# Initial Installation
- ROS
    - [ROS INSTALL LINK](http://wiki.ros.org/ROS/Installation)
- Gazebo
    - `sudo apt install gazebo`

# Commands
### Building
- Use the catkin build system to "build" the programs
    - `catkin_make`
- Add all the environment variables in this file to our current list of environment variables
    - `source devel/setup.sh`
- Also add this TURTLEBOT3 model environment variable
    - `export TURTLEBOT3_MODEL=burger`

### Running
- Launch the Gazebo world to visualize the robot and its environment
    - `roslaunch turtlebot3_gazebo turtlebot3_house.launch`
- Control the robot using your keyboard
    - `roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch`
- Have the robot autonomously drive itself
    - `roslaunch turtlebot3_gazebo turtlebot3_simulation.launch`
- Have the robot map its world
    - `roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping`

