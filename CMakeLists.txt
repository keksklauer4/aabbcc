cmake_minimum_required(VERSION 3.7)

project(aabbcc)

enable_language(C CXX)
set(CMAKE_CXX_STANDARD 20)
set(CXX_STANDARD_REQUIRED ON)
set(CMAKE_BUILD_TYPE Release)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_library(aabbcc src/AABB.cc)

target_include_directories(aabbcc PRIVATE src/)

set(AABBCC_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include/ CACHE INTERNAL "")
