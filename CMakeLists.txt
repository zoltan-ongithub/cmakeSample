cmake_minimum_required(VERSION 3.15)
project(cmakeSampleProject)

set(CMAKE_CXX_STANDARD 14)

add_executable(cmakeSampleProject main.cpp)

add_library(samplelib SHARED
    samplelib.cpp
    )

set(HEADER_FILES cmakesample.h)

install(TARGETS cmakeSampleProject DESTINATION bin)
install(TARGETS samplelib DESTINATION lib)
install(FILES ${HEADER_FILES} DESTINATION include)

