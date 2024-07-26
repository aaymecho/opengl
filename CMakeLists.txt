cmake_minimum_required(VERSION 3.10)
project(OpenGLTriangle)

set(CMAKE_CXX_STANDARD 14)

find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)
find_package(glfw3 REQUIRED)

add_executable(OpenGLTriangle main.cpp)

target_link_libraries(OpenGLTriangle ${OPENGL_LIBRARIES} GLEW::GLEW glfw)
