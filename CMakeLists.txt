cmake_minimum_required(VERSION 3.13)

project(example)

enable_testing()

add_subdirectory(googletest)

add_library(example STATIC example.cpp example.h)

add_subdirectory(tests)
