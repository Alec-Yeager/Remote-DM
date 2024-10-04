cmake_minimum_required(VERSION 3.30)
project(remote-dm)

set(CMAKE_CXX_STANDARD           20)
set(CMAKE_CXX_STANDARD_REQUIRED YES)
set(CMAKE_CXX_EXTENSIONS        OFF)

find_package(Qt6 REQUIRED COMPONENTS Widgets)
qt_standard_project_setup

qt_add_executable(remote-dm-server src/main.cpp)

target_link_libaries(remote-dm-server PRIVATE Qt6::Core)
