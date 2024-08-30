cmake_minimum_required(VERSION 3.20)
project(c-library)

add_library(${PROJECT_NAME} STATIC src/sample_lib.cpp)

target_include_directories(${PROJECT_NAME}
    PUBLIC include/
    PRIVATE src/
)
