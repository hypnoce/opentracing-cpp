cmake_minimum_required(VERSION 3.0)
enable_testing()

project(opentracing-cpp)

set(OPENTRACING_ABI_VERSION "1")

SET(CPACK_PACKAGE_DESCRIPTION_SUMMARY "C++ implementation of the OpenTracing API")
SET(CPACK_PACKAGE_VENDOR "opentracing.io")
SET(CPACK_PACKAGE_DESCRIPTION_FILE "${CMAKE_CURRENT_SOURCE_DIR}/README.md")
SET(CPACK_RESOURCE_FILE_LICENSE "${CMAKE_CURRENT_SOURCE_DIR}/LICENSE")

SET(CPACK_PACKAGE_VERSION_MAJOR "0")
SET(CPACK_PACKAGE_VERSION_MINOR "1")
SET(CPACK_PACKAGE_VERSION_PATCH "0")
include(CPack)

add_subdirectory(c++11)