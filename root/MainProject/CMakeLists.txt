cmake_minimum_required(VERSION 3.24)
include_directories(${MyProject_SOURCE_DIR}/MainProject/inc)
# I assume you want to use LibProject as a library in MainProject.
include_directories(${MyProject_SOURCE_DIR}/LibProject/inc)
link_directories(${MyProject_SOURCE_DIR}/LibProject/src)
add_executable(MainProject src/main.cpp)
target_link_libraries(MainProject LibProject)
