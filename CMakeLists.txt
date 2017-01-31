cmake_minimum_required (VERSION 2.8.11)
project (Pong)

# La versión
set (Pong_VERSION_MAJOR 0)
set (Pong_VERSION_MINOR 1)
set (Pong_VERSION_PATCH 0)

# configure a header file to pass some of the CMake settings
# to the source code
configure_file (
  "${PROJECT_SOURCE_DIR}/in/PongConfig.h.in"
  "${PROJECT_BINARY_DIR}/PongConfig.h"
)

# add the binary tree to the search path for include files
# so that we will find TutorialConfig.h
include_directories("${PROJECT_BINARY_DIR}")

add_subdirectory(Pong)
