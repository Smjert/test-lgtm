cmake_minimum_required(VERSION 3.13.0)

project(test-lgtm)

add_executable(test-lgtm main.cpp)

add_library(test-lgtm-lib blah/lib.cpp)
add_library(test-lgtm-lib2 blah/a/lib2.cpp)

target_link_libraries(test-lgtm PRIVATE test-lgtm-lib test-lgtm-lib2)
