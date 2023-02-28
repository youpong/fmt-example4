# README

This is an example of the {fmt} library. 
Using conan for dependency management.

## Dependencies

* cmake 3.22 or later
* conan 2.0.0 or later

## How to build

```bash
$ conan install . --output-folder=build --build=missing
$ cd build
$ cmake .. -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Release
$ cmake --build build
```

# License

This project is distributed under the MIT license.
