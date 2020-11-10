cmake_minimum_required(VERSION 3.13)

add_executable(Tests tests.cpp)

target_link_libraries( Tests PUBLIC
	gtest_main
	example
)

add_test(
	NAME Tests
	COMMAND Tests
)
