cmake_minimum_required(VERSION 2.8)


project(OPTICAL_FLOW)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(Optical_Flow_CPU Optical_Flow_CPU.cpp)

target_link_libraries(Optical_Flow_CPU ${OpenCV_LIBS})
