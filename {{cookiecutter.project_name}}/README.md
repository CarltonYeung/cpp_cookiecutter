# {{cookiecutter.project_name}}
This project was generated with [C++ Cookiecutter](https://github.com/CarltonYeung/cpp_cookiecutter).

<br>

## Prerequisites
---
- C++17
- [CMake >= 3.14](https://cmake.org/install/)

<br>

## Build
---
```
cd {{cookiecutter.project_name}}
cmake -S . -B build
cmake --build build
```

## Test
---
```
cd build
ctest
```
