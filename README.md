# hpe_ros_msgs


ROS package containing custom ROS messages for human pose estimation. 

# Depends on: 

`vision_msgs` modified so that contain `Point2D.msg` as found [here](https://github.com/fzoric8/vision_msgs/tree/noetic-devel). 




# msg contained 

Pkg contains following messages: 
 * `ArmCmd.msg` -> contains shoulder roll, pitch, yaw and elbow angle 
 * `TorsoJointPositions.msg` -> contains vectors from camera origin to the body keypoint 

