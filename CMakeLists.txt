cmake_minimum_required(VERSION 3.26.4)

project(
    rpmalloc
    VERSION 1.4.4.1
    LANGUAGES C
)

file(GLOB_RECURSE SOURCES rpmalloc/*.c)

add_library(rpmalloc SHARED ${SOURCES})
target_include_directories(rpmalloc PUBLIC ./rpmalloc)