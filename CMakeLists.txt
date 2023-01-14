cmake_minimum_required(VERSION 3.14)

project(LibMatematicas LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(LibMatematicas SHARED
  LibMatematicas_global.h
  matematicas.cpp
  matematicas.h
)

target_compile_definitions(LibMatematicas PRIVATE LIBMATEMATICAS_LIBRARY)
