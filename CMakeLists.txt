cmake_minimum_required(VERSION 3.5)

#################################################################
# find_package(Boost REQUIRED COMPONENTS unit_test_framework)
include_directories("${PROJECT_SOURCE_DIR}/ParallelLib/include")
set(PARALLEL_LIB_SOURCES ${PROJECT_SOURCE_DIR}/ParallelLib/ParallelLib.cpp)
set(PARALLEL_LIB ParallelLib)
add_library(ParallelLib SHARED ${PARALLEL_LIB_SOURCES})

