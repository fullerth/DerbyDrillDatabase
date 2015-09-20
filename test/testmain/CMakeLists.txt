set(TEST_SOURCES
    test_main.cpp)

add_executable(testmain ${TEST_SOURCES})

include_directories(../../lib/gtest/include)

install(TARGETS testmain DESTINATION bin)
