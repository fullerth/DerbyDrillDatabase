## CMakeLists.txt
cmake_minimum_required(VERSION 2.8.7)
project(GmockSetup)

## Project Configuration
add_definitions(-std=c++11)
add_definitions(-Wall)
add_definitions(-Werror)
include(CTest)

set(TEST_EXE_PATH /home/pthrill/Projects/GmockSetup/build/test/)

## Directories to add to build
add_subdirectory(lib/gmock)

add_subdirectory(src/main)
add_subdirectory(test/testmain)
add_test(NAME AllTestsInMain
    COMMAND ${TEST_EXE_PATH}testmain/testmain)

add_subdirectory(src/foolib)
add_subdirectory(test/testfoo)
add_test(NAME AllTestsInFoo
    COMMAND ${TEST_EXE_PATH}testfoo/testfoo)


# Project Source
set(MAIN_SOURCES
    src/main/main.cpp
    src/foolib/foo.cpp)
include_directories(
    src/foolib/include)

add_executable(GmockSetup
    ${MAIN_SOURCES}
	       )
