cmake_minimum_required (VERSION 2.8.11)
project (Pong)

# "TRUE to build SFML as shared libraries, FALSE to build it as static libraries"
set(BUILD_SHARED_LIBS TRUE)

# La versión
set (Pong_VERSION_MAJOR 0)
set (Pong_VERSION_MINOR 1)
set (Pong_VERSION_PATCH 0)

# La versión se pasa a un templete de header para que el código lo pueda usar
configure_file (
  "${PROJECT_SOURCE_DIR}/in/PongConfig.h.in"
  "${PROJECT_BINARY_DIR}/PongConfig.h"
)

include_directories ("${PROJECT_SOURCE_DIR}/include")

# Hay que agregar el directorio del binario a la búsqueda de includes para que
# pueda conseguir PongConfig.h
include_directories("${PROJECT_BINARY_DIR}")

add_subdirectory(Pong)
