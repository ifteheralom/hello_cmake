cmake_minimum_required(VERSION 2.4)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

project(hello_world)

include_directories(include)
file(GLOB_RECURSE SOURCES "include/*.h" "src/*.cpp")

add_executable(app src/main.cpp src/foo.cpp)
 
