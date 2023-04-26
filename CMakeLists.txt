cmake_minimum_required(VERSION 3.14...3.26)
	
project(example LANGUAGES CXX)

set(CMAKE_BUILD_TYPE Release)

enable_testing()

find_package(GTest REQUIRED)

include(GoogleTest)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include(CMakePrintHelpers)
cmake_print_variables(CMAKE_CXX_COMPILER_ID)
cmake_print_variables(CMAKE_CXX_COMPILER_VERSION)

add_subdirectory(projectname)