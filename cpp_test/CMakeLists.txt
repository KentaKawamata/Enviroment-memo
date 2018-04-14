cmake_minimum_required(VERSION  3.5)

project(running CXX)

#find the opencv2 liblary
find_package(OpenCV REQUIRED)

add_executable(running main.cpp)
target_link_libraries(running ${OpenCV_LIBS})
add_definitions("-std=c++14")
