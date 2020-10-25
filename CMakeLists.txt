cmake_minimum_required(VERSION 3.15)
project(cmakeSampleProject)

set(CMAKE_CXX_STANDARD 14)

add_executable(cmakeSampleProject main.cpp)
install(TARGETS cmakeSampleProject DESTINATION bin)

