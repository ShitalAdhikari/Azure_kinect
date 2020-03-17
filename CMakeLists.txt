cmake_minimum_required(VERSION 2.8)
project(AzureKinect)
find_package(OpenCV REQUIRED)
find_package(k4a REQUIRED)

add_executable(AzureKinect main.cpp)
target_link_libraries(AzureKinect ${OpenCV_LIBS} k4a::k4a )
#target_link_libraries(AzureKinect PRIVATE k4a::k4a)
