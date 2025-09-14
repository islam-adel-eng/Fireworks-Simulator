cmake_minimum_required(VERSION 3.26)
project(main C CXX)

find_package(SDL3 REQUIRED)

add_executable(main)

target_sources(main
PRIVATE
    "src/main.c"
)

target_link_libraries(main SDL3::SDL3)