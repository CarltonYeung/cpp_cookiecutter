cmake_minimum_required(VERSION 3.10)

# set the project name
project({{cookiecutter.project_name}})

# specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# generate compile_commands.json
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

# set executables output location
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})

# add subdirectories
add_subdirectory(src)

# enable testing
enable_testing()
add_subdirectory(tests)
