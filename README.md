🤖 Line Following Robot (ROS2)
This is a ROS2-based simulation of a line-following robot built using Gazebo and OpenCV. The robot follows a predefined path by detecting and tracking colored lines via HSV color segmentation for real-time object detection.

🧠 Features
✅ Built with ROS2 Humble

🎥 Real-time camera feed visualization

🧪 Line detection using HSV color space

⚙️ Simple control using joint commands

🧰 Uses OpenCV for image processing

🛠 Simulated in Gazebo Classic

🚀 Getting Started
1. Set the Gazebo Model Path
Before launching the robot, set the Gazebo model path:
export GAZEBO_MODEL_PATH=/home/esayas/Desktop/line_follower/src/simple_robot_description/models:$GAZEBO_MODEL_PATH

3. Launch the Simulation
Start the robot simulation in Gazebo:
ros2 launch simple_robot_description gazebo.launch.py

3. View the Camera Feed
Use the image_tools package to view the robot's camera feed:
ros2 run image_tools showimage --ros-args --remap image:=/camera1/image_raw

4. Start the Line-Following Behavior
Run the joint commander to initiate the line-following logic:
ros2 run simple_robot_description joint_commander

🛠 Dependencies
ROS2 (Foxy, Humble, or compatible versions)
OpenCV (Python bindings)
Gazebo Classic
image_tools package

Screenshots
![Screenshot 2025-04-24 085453](https://github.com/user-attachments/assets/95992e80-db05-4845-98a5-9c68c69936b6)
![Screenshot 2025-04-24 085427](https://github.com/user-attachments/assets/59003a99-af6e-4aeb-87e9-2c92a8ca52b3)
