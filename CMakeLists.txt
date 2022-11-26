cmake_minimum_required(VERSION 2.8.9)

project(Logger)

set(CMAKE_BUILD_TYPE Debug)
# specify the C++ standard
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(INSTALL_NAME_DIR ${CMAKE_CURRENT_BINARY_DIR})

#Bring the headers into the project
include_directories(include)

file(GLOB SOURCES  ${CMAKE_CURRENT_SOURCE_DIR}/Logger.cpp)

add_executable(TestLogger ${CMAKE_CURRENT_SOURCE_DIR}/Logger.cpp)
