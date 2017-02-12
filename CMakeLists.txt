# Configuration largely taken from https://cmake.org/cmake-tutorial/
# and from http://derekmolloy.ie/hello-world-introductions-to-cmake/

cmake_minimum_required (VERSION 2.6)
project (Polynomial)

# The version number.
set (Polynomial_VERSION_MAJOR 0)
set (Polynomial_VERSION_MINOR 1)

include_directories(include)
file(GLOB SOURCES "src/*.cpp")
add_executable(polynomial ${SOURCES})

enable_testing()
add_subdirectory(test)
