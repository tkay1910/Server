cmake_minimum_required(VERSION 3.0.0)
project(server VERSION 0.1.0)

add_subdirectory ("Library")

include(CTest)
enable_testing()

add_executable(server main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
