# https://github.com/google/googletest/tree/master/googletest#incorporating-into-an-existing-cmake-project
include(FetchContent)
FetchContent_Declare(
  googletest
  URL https://github.com/google/googletest/archive/96f4ce02a3a78d63981c67acbd368945d11d7d70.zip
)

FetchContent_MakeAvailable(googletest)

# add subdirectories
add_subdirectory(unittests)
