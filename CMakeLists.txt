cmake_minimum_required(VERSION 3.12.4)

set(CMAKE_C_COMPILER "/usr/bin/clang-9")
set(CMAKE_CXX_COMPILER "/usr/bin/clang++-9")

project(cpp_project)

# Set C++ standard to C++17
set(CMAKE_CXX_STANDARD 17)

# Set standard library to libc++
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -stdlib=libc++")

include_directories(src)

add_subdirectory(src)
add_subdirectory(test)
add_subdirectory(external/googletest)