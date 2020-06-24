cmake_minimum_required(VERSION 3.8)

set(CMAKE_C_STANDARD 99)
include_directories(include)

# Find all source file in src, and set to HELLOWORLD_SRCS
aux_source_directory(src HELLOWORLD_SRCS)

add_library(helloworld ${HELLOWORLD_SRCS})
