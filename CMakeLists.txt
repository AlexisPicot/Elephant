cmake_minimum_required(VERSION 3.8)
project(Elephant)

set(CMAKE_C_STANDARD 99)

set(SOURCE_FILES gpu.h gpu.c pipeline-graphic.c)

add_executable(Elephant ${SOURCE_FILES} )
target_link_libraries(Elephant m pthread)