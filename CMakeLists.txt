cmake_minimum_required(VERSION 3.5)

set(QUICK_START_VERSION_MAJOR 1)
set(QUICK_START_VERSION_MINOR 0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

#################################################################
# find_package(Boost REQUIRED COMPONENTS unit_test_framework)
set(PARALLEL_LIB_SOURCES ${PROJECT_SOURCE_DIR}/ParallelLib/ParallelLib.cpp)
include_directories("${PROJECT_SOURCE_DIR}/ParallelLib/include")
add_library(ParallelLib SHARED ${PARALLEL_LIB_SOURCES})

