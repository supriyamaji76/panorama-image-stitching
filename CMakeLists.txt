cmake_minimum_required(VERSION 3.10)

project(panorama)

find_package(OpenCV REQUIRED)

add_executable(panorama src/panorama.cpp)

target_link_libraries(panorama ${OpenCV_LIBS})