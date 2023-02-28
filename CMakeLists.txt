cmake_minimum_required(VERSION 3.22)

project(fmt-example4)

find_package(fmt REQUIRED)

add_executable(main main.cc)
target_link_libraries(main fmt::fmt)

target_compile_features(main PRIVATE cxx_std_20)

target_compile_options(main PRIVATE
  "-Wall;-Wextra;-Wpedantic"
)
