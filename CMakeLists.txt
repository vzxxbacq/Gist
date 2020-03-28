cmake_minimum_required(VERSION 3.10)
project(Gist)
set(CMAKE_CXX_STANDARD 14)

include_directories(src)
set(SOURCE_FILES src/Gist.cpp)

add_library(Gist ${SOURCE_FILES})