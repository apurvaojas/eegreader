cmake_minimum_required(VERSION 3.0.0)
project(eegreader VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(eegreader src/eegreader.c)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
set(EXECUTABLE_OUTPUT_PATH ./bin)
include(CPack)
