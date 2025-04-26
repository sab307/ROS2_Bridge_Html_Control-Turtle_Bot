##Setup the Gazebo environment and launch the respective file.
```bash
source /usr/share/gazebo/setup.bash
source turtlebot3_ws/install/setup.sh 
export TURTLEBOT3_MODEL=burger
ros2 launch turtlebot3_gazebo empty_world.launch.py
```

## Setup the Turtle Bot3 package (Ros2 Humble) and Compile
```bash
mkdir -p ~/turtlebot3_ws/src
cd ~/turtlebot3_ws/src/
git clone -b humble-devel https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
cd ~/turtlebot3_ws && rosdep install --from-paths src --ignore-src -r -y
colcon build --symlink-install
source install/setup.bash
```

Now install the relevant rosbridge library
```bash
sudo apt install ros-humble-rosbridge-server
```

Launch the respective rosbridge file.
```bash
ros2 launch rosbridge_server rosbridge_websocket.launch.xml
```
After launching the above command, open the html file in the web browser
to control the turtlebot3.