## CMakeLists.txt
cmake_minimum_required(VERSION 2.6.2)
project(Derby_Drill_Database)
set(gtest_dir "lib/googletest-release-1.7.0")
add_subdirectory("lib/gmock")
set(DRILL_SOURCES
    main.cpp)

# Google Test
include_directories("lib/gtest/include")

add_executable(derby_drill_database
	       ${DRILL_SOURCES})

