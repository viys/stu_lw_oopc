cmake_minimum_required(VERSION 3.0.0)

set(CMAKE_C_FLAGS "-std=c99")

project(lw_oopc)

file(GLOB_RECURSE SRC ${CMAKE_CURRENT_SOURCE_DIR}/app/*.c)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/app/)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/app/lw_oopc)

add_executable(lw_oopc ${SRC})