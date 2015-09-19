## CMakeLists.txt
cmake_minimum_required(VERSION 2.6.2)
project(Derby_Drill_Database)
set(DRILL_SOURCES
    main.cpp)

# Google Test
include_directories("~/googletest/googletest")

add_executable(derby_drill_database
	       ${DRILL_SOURCES})

