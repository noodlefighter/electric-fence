cmake_minimum_required(VERSION 3.1)
project(efence)

add_definitions(-g -DUSE_SEMAPHORE -fPIC)

add_library(efence efence.c page.c print.c)
add_library(efence::efence ALIAS efence)
