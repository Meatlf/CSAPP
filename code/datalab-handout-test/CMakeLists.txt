# set minimum cmake version
cmake_minimum_required(VERSION 3.5 FATAL_ERROR)

# project name and language
project(chapter01 LANGUAGES CXX)

#dubug 模式
set (CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -g")

# add_executable(print_test print_test.cpp)
# add_executable(polynomial polynomial.cpp)
add_executable(project01 01-复杂度1-最大子列和问题.cpp)
add_executable(project02 01-复杂度2-MaximumSubsequenceSum.cpp)