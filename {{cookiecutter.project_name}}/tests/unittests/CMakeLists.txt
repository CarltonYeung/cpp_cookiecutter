# https://github.com/google/googletest/tree/master/googletest#incorporating-into-an-existing-cmake-project

# add unittest executable
add_executable(
    unittests
    example_test.cpp
)

target_link_libraries(
    unittests
    gtest
    gtest_main
    pthread
)

include(GoogleTest)
gtest_discover_tests(unittests)
