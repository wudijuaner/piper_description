cmake_minimum_required(VERSION 3.0.2)
project(piper_description)

find_package(catkin REQUIRED COMPONENTS
  urdf
  rviz
  robot_state_publisher
  joint_state_publisher
  joint_state_publisher_gui
)

catkin_package()

install(DIRECTORY launch urdf meshes
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)