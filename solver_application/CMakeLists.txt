cmake_minimum_required(VERSION 3.10)
project(solver LANGUAGES CXX)

add_executable(solve
    equation.cpp
)

target_link_libraries(solve
    PRIVATE
    formatter_ex
    solver_lib
)
