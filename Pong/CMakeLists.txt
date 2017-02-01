# Ejecutable de Pong, solo requiere main.cpp
add_executable (Pong main.cpp)

target_link_libraries(Pong
  debug "${PROJECT_SOURCE_DIR}/libs/vc140-win32-debug/sfml-audio-d.lib"
  debug "${PROJECT_SOURCE_DIR}/libs/vc140-win32-debug/sfml-graphics-d.lib"
  debug "${PROJECT_SOURCE_DIR}/libs/vc140-win32-debug/sfml-main-d.lib"
  debug "${PROJECT_SOURCE_DIR}/libs/vc140-win32-debug/sfml-network-d.lib"
  debug "${PROJECT_SOURCE_DIR}/libs/vc140-win32-debug/sfml-system-d.lib"
  debug "${PROJECT_SOURCE_DIR}/libs/vc140-win32-debug/sfml-window-d.lib"
  optimized "${PROJECT_SOURCE_DIR}/libs/vc140-win32-release/sfml-audio.lib"
  optimized "${PROJECT_SOURCE_DIR}/libs/vc140-win32-release/sfml-graphics.lib"
  optimized "${PROJECT_SOURCE_DIR}/libs/vc140-win32-release/sfml-main.lib"
  optimized "${PROJECT_SOURCE_DIR}/libs/vc140-win32-release/sfml-network.lib"
  optimized "${PROJECT_SOURCE_DIR}/libs/vc140-win32-release/sfml-system.lib"
  optimized "${PROJECT_SOURCE_DIR}/libs/vc140-win32-release/sfml-window.lib"
)
