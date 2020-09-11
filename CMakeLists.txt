cmake_minimum_required(VERSION 3.10)

project(fib-container CXX)

add_executable(fib-container src/main.cpp)

find_package(fmt CONFIG REQUIRED)
find_package(cppitertools CONFIG REQUIRED)

target_link_libraries(fib-container
  PRIVATE
    fmt::fmt
    cppitertools::cppitertools)
    