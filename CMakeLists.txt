cmake_minimum_required(VERSION 3.13)

project(fibonacci CXX)

add_executable(fibonacci src/main.cpp)

find_package(fmt CONFIG REQUIRED)
find_package(cppitertools CONFIG REQUIRED)

target_link_libraries(fibonacci
  PRIVATE
    fmt::fmt
    cppitertools::cppitertools)
    