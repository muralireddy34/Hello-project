cmake_minimum_required(VERSION 3.24)
# Notice name prefix of this variable, set by CMake according
# to value given with "project()" in the root CMakeLists.txt.
include_directories(${MyProject_SOURCE_DIR}/LibProject/inc)
add_library(LibProject src/test.cpp)
