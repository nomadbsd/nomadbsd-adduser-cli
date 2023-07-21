# VERSION
cmake_minimum_required(VERSION 3.15)

# PROJECT 
project(nomadbsd-adduser-cli)

# SOURCE CODE DIRECTORY
add_subdirectory(src)

# C STANDARD
set(CMAKE_C_STANDARD 17)
set(CMAKE_C_STANDARD_REQUIRED True)