cmake_minimum_required(VERSION 3.10)
project(LogSvcExampleApp)

#----------------------------------------------------------------------------
# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

#----------------------------------------------------------------------------
# Define project directories
set(PROJECT_SOURCE_DIR "${CMAKE_SOURCE_DIR}")
set(INCLUDE_DIR "${PROJECT_SOURCE_DIR}/include")
set(SRC_DIR "${PROJECT_SOURCE_DIR}/src")
set(EXAMPLES_DIR "${PROJECT_SOURCE_DIR}/examples")
set(TESTS_DIR "${PROJECT_SOURCE_DIR}/tests")
set(EXTERNALS_DIR "${PROJECT_SOURCE_DIR}/externals")

#----------------------------------------------------------------------------
# Add subdirectories
add_subdirectory(${SRC_DIR})
add_subdirectory(${EXAMPLES_DIR})
add_subdirectory(${TESTS_DIR})
