cmake_minimum_required(VERSION 3.16)

project(session1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Catch2 2 REQUIRED)
add_executable(test test.cc)
target_link_libraries(test Catch2::Catch2)
