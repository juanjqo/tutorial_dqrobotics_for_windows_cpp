cmake_minimum_required(VERSION 3.5)

project(hello_world LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(DQROBOTICS_DIR ${CMAKE_CURRENT_SOURCE_DIR}/../../cpp/)
include(${CMAKE_CURRENT_SOURCE_DIR}/../../dependencies.cmake)

add_executable(${CMAKE_PROJECT_NAME} main.cpp)

target_link_libraries(${CMAKE_PROJECT_NAME} dqrobotics)
