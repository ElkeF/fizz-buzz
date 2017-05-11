# stop if CMake version is below 2.8
cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

# project name
project(fizz-buzz)

# this is a Fortran and C++ project
enable_language(CXX)
enable_language(Fortran)

# specify where to place binaries and libraries
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY
    ${CMAKE_BINARY_DIR}/bin
    )
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY
    ${CMAKE_BINARY_DIR}/lib
    )

# process src/CMakeLists.txt
add_subdirectory(src)


