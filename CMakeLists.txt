cmake_minimum_required(VERSION 3.10)

project(learnopengl VERSION 0.1.0)

add_subdirectory(glad)
add_subdirectory(glfw)
add_subdirectory(learnopengl)


target_include_directories(learnopengl PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/glew/include)


# target_include_directories(learnopengl PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/includes/glad)
# target_include_directories(learnopengl PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/includes/KHR)

# add_library(GLAD "src/glad.c")