cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
project(PathCornerCreator)
#find_package(PCL 1.7 REQUIRED)
find_package(catkin REQUIRED COMPONENTS roscpp)




catkin_package()
include_directories(${catkin_INCLUDE_DIRS})
link_directories(${catkin_LIBRARY_DIRS})
add_definitions(${catkin_DEFINITIONS})
add_executable (PathCornerCreator src/topictest.cpp)
#add_dependencies(${PROJECT_NAME} ${${PROJECT_NAME}_EXPORTED_TARGETS})

target_link_libraries (PathCornerCreator ${catkin_LIBRARIES})

