cmake_minimum_required(VERSION 3.15)
project(raytracer VERSION 0.1.0)
set(CMAKE_CXX_STANDARD 14)

include(CTest)
enable_testing()


aux_source_directory(src SRC)

add_executable(raytracer ${SRC})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
