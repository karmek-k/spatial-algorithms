cmake_minimum_required(VERSION 3.20)
project(spatial_algorithms C)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

if(CMAKE_C_COMPILER_ID MATCHES "GNU|Clang")
    add_compile_options(-Wall -Wextra)
endif()

add_subdirectory(lib)
add_subdirectory(programs/example)
add_subdirectory(programs/point_side)
