# CMake version
cmake_minimum_required(VERSION 3.8.2 FATAL_ERROR)

set(CMAKE_CXX_STANDARD 17)

# Declare project
project(MuZero)

# Set output directories
set(DEFAULT_CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_LIBRARY_OUTPUT_DIRECTORY})
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/lib)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/lib)

# Includes
include_directories(include)

# Sub directories
add_subdirectory(src)

