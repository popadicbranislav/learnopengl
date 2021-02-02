cmake_minimum_required(VERSION 3.10)

project(learnopengl VERSION 0.1.0)

add_subdirectory(glad)
add_subdirectory(glfw)
add_subdirectory(assimp)
add_subdirectory(getting_started)
add_subdirectory(lighting)
add_subdirectory(model_loading)

target_include_directories(getting_started PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/glew/include)
target_include_directories(lighting PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/glew/include)
target_include_directories(model_loading PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/glew/include)