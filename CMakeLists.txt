cmake_minimum_required(VERSION 3.10)

project(learnopengl VERSION 0.1.0)

add_subdirectory(glad)
add_subdirectory(glfw)
add_subdirectory(getting_started)

target_include_directories(getting_started PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/glew/include)