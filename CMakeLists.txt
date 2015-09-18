## CMakeLists.txt
cmake_minimum_required(VERSION 2.6.2)
project(Derby_Drill_Database)
set(DRILL_SOURCES
    main.cpp)
set(GTEST_LIB
    ../gtest)
add_executable(derby_drill_database
	       ${DRILL_SOURCES})



#option(drills_build_tests "Build all of the Derby Drill Database's unit tests." OFF)
#include_directories("/usr/local/include")
#link_directories("/usr/local/lib")
#set(drills_SOURCES
#    main.cpp
#    html_parser.h
#    http_fetch.h)
#add_executable(foo ${foo_SOURCES})
#if (foo_build_tests)
#enable_testing()
#add_executable(html_parser_test
#html_parser_test.cc
#html_parser.h
#http_fetch.h)
#target_link_libraries(html_parser_test
#pthread)
#target_link_libraries(html_parser_test
#gmock
#gmock_main)
#target_link_libraries(html_parser_test
#gtest
#gtest_main)
#add_test(html-tests html_parser_test)
#endif()
