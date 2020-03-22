cmake_minimum_required(VERSION 3.0.0)
project(chapter10 VERSION 0.1.0)

include(CTest)
enable_testing()

#dubug 模式
# set (CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -g")
set (CMAKE_C_FLAGS  "${CMAKE_C_FLAGS} -g")

# 添加头文件路径
# include_directories("${PROJECT_SOURCE_DIR}/exercise1")

add_executable(show-bytes ./show-bytes.c)
# add_executable(test_exercise2 ./exercise2.cpp)

# 添加子目录
# add_subdirectory(exercise1)

# 添加库
# target_link_libraries(test_exercise1 exercise1)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
