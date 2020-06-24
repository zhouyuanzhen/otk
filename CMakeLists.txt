cmake_minimum_required(VERSION 3.8)
project(otk)
set(CMAKE_C_STANDARD 99)

set(DemoApp demo-otk)
set(SOURCE_FILES demo/demo.c)

include_directories(helloworld/include)
add_executable(${DemoApp} ${SOURCE_FILES})
target_link_libraries (${DemoApp} helloworld)

add_subdirectory (helloworld)
