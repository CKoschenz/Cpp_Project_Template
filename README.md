# C++ Project Temnplate

This C++ Project Templates contains a start-up configuration for CMake, Conan and ...

## Required software

- CMake 3.>16
- Conan 2.>0

## Quickstart

Build

```shell
$ conan install . --output-folder=build --build=missing
$ cmake -S . -B build -DCMAKE_TOOLCHAIN_FILE=build/conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Release
$ cmake --build build
```

For Debugging

```shell
$ conan install . --output-folder=build --build=missing -s build_type=Debug
```