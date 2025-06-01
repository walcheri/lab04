cmake_minimum_required(VERSION 3.10)
project(formatter_ex LANGUAGES CXX)

add_library(formatter_ex STATIC 
    formatter_ex.cpp
    formatter_ex.h
)

target_include_directories(formatter_ex
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
    ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_lib
)

target_link_libraries(formatter_ex 
    PUBLIC 
    formatter
)
