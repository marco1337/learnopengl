cmake_minimum_required(VERSION 3.0.0)
project(my_opengl_project)

set(SOURCES
    src/main.cpp
    src/glad.c
)

add_executable(my_opengl_project ${SOURCES})

target_include_directories(my_opengl_project
    PRIVATE
	${PROJECT_SOURCE_DIR}/include
)

target_link_libraries(my_opengl_project glfw)

