## CMakeLists.txt
cmake_minimum_required(VERSION 2.8.7)
project(GmockSetup)

#set(CMAKE_INCLUDE_CURRENT_DIR ON)

add_subdirectory(lib/gmock)
add_subdirectory(main)
add_subdirectory(test/testmain)
add_subdirectory(foolib)

#Gmock Setup
set(MAIN_SOURCES
    main/main.cpp)

add_executable(GmockSetup
    ${MAIN_SOURCES}
	       )
