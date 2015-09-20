## CMakeLists.txt
cmake_minimum_required(VERSION 2.8.7)
project(Derby_Drill_Database)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

add_subdirectory(lib/gmock)
add_subdirectory(main)
add_subdirectory(test/testmain)
set(DRILL_SOURCES
    main/main.cpp)

# Google Test
include_directories("lib/gtest/include")
add_executable(derby_drill_database
	       ${DRILL_SOURCES})

