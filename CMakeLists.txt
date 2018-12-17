cmake_minimum_required(VERSION 3.13)

project(LearnOpenGL)

set(CMAKE_CXX_STANDARD 14)

find_package(glad CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)

add_executable(LearnOpenGL 2_hello_triangle.cpp)

target_link_libraries(LearnOpenGL PRIVATE glfw)
target_link_libraries(LearnOpenGL PRIVATE glad::glad)
