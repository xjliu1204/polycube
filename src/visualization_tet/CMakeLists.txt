#cmake_minimum_required(VERSION 2.8)
PROJECT(visual_tet)
FIND_PACKAGE(VTK)
#INCLUDE(${VTK_USE_FILE})
set(CMAKE_DEBUG_POSTFIX "d")
#SET(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})
set(CMAKE_CXX_FLAGS "-std=c++0x ${CMAKE_CXX_FLAGS}")
include_directories(/usr/include/vtk-5.8)
ADD_SUBDIRECTORY(./configure)
ADD_SUBDIRECTORY(./call_back)
ADD_SUBDIRECTORY(./io)
ADD_SUBDIRECTORY(./widget)
ADD_SUBDIRECTORY(./vtk_operate)
ADD_SUBDIRECTORY(./side_bar)
ADD_SUBDIRECTORY(./main_win)
ADD_SUBDIRECTORY(./main)
