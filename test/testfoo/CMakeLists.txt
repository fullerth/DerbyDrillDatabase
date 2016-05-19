set(TEST_SOURCES
    main.cpp
    test_foo.cpp
    ../../foolib/foo.cpp)

add_executable(testfoo ${TEST_SOURCES})

target_link_libraries(testfoo
	gtest
	)

include_directories(
    ../../lib/gtest/include
    ../../foolib/include
    )

