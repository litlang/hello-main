cmake_minimum_required(VERSION 3.15)

project(hello)

file(GLOB_RECURSE SOURCES src/*.cxx)
add_executable(${PROJECT_NAME} ${SOURCES})

install(TARGETS ${PROJECT_NAME} RUNTIME DESTINATION bin)
