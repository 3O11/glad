cmake_minimum_required(VERSION 3.20)

project(glad
    LANGUAGES C
)

add_library(glad STATIC
    "include/KHR/khrplatform.h"
    "include/glad/gl.h"
    "src/gl.c"
)

target_include_directories(glad
    PUBLIC
    "include"
)
