cmake_minimum_required(VERSION 3.18.0 FATAL_ERROR)
project(test1)
find_package(PCL 1.9.1 REQUIRED COMPONENTS)
include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})
add_executable(test1 test1.cpp)
target_link_libraries(test1 ${PCL_LIBRARIES})