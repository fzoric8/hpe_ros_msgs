cmake_minimum_required(VERSION 3.0.2)
project(hpe_ros_msgs)


## Compile as C++11, supported in ROS Kinetic and newer
add_compile_options(-std=c++11)

## Find catkin macros and libraries
find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
  sensor_msgs
  vision_msgs
  message_generation
)

add_message_files(
  FILES
  TorsoJointPositions.msg
  JointArmCmd.msg
  CartesianArmCmd.msg
  EstLinkLengths.msg
  HumanPose2D.msg
  HandPose2D.msg
  HumanPose3D.msg
  HandPose3D.msg
)

generate_messages(
  DEPENDENCIES
  std_msgs
  geometry_msgs
  vision_msgs
)

catkin_package(
  CATKIN_DEPENDS roscpp rospy std_msgs vision_msgs message_runtime
)
