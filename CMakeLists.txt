cmake_minimum_required(VERSION 3.5.2)
project(kilo)

set(CMAKE_CXX_STANDARD 14)

set(SOURCE_FILES main.cpp)
set(EXECUTABLE_OUTPUT_PATH   "bin")
add_executable(kilo ${SOURCE_FILES})

set(gtest_INCLUDE_DIR ./../googletest-master)
include_directories(gtest_INCLUDE_DIR/include gtest_INCLUDE_DIR)
include_directories(lib test bin)

