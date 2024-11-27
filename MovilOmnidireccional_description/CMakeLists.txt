cmake_minimum_required(VERSION 3.8)
project(MovilOmnidireccional_description)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

# find dependencies
find_package(ament_cmake REQUIRED)
# uncomment the following section in order to fill in
# further dependencies manually.
# find_package(<dependency> REQUIRED)
# find dependencies
find_package(ament_cmake REQUIRED)
# find dependencies
find_package(ament_cmake REQUIRED)
#find_package(ament_cmake_python REQUIRED) #for python scripts
find_package(rclcpp REQUIRED)
#find_package(rclpy REQUIRED) #for python scripts
find_package(geometry_msgs REQUIRED)
#find_package(nav_msgs REQUIRED)
find_package(tf2 REQUIRED)
find_package(std_msgs REQUIRED)
find_package(control_msgs REQUIRED) #for ros control
find_package(rclcpp_action REQUIRED) #for ros control actions

install(
  DIRECTORY launch meshes rviz urdf
  DESTINATION share/${PROJECT_NAME}/
)

ament_package()
