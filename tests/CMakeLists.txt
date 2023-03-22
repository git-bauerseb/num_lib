enable_testing()

add_executable(
    simple_test
    SimpleTest.cpp
)

target_link_libraries(
    simple_test
    GTest::gtest_main
)

include(GoogleTest)
gtest_discover_tests(simple_test)
