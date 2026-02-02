cmake_minimum_required(VERSION 3.10)

project(MikkTSpace C)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_library(${PROJECT_NAME} STATIC
    mikktspace.h
    mikktspace.c
)

target_include_directories(${PROJECT_NAME}
PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)
