set(TEST_SOURCES
    test_main.cpp
    main.cpp)

add_executable(testmain ${TEST_SOURCES})

target_link_libraries(testmain
	gtest
	)

include_directories(../../lib/gtest/include)

install(TARGETS testmain)
