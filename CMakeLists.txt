cmake_minimum_required(VERSION 2.8.0)

project(vtable)

add_executable(vtable_gen ${CMAKE_SOURCE_DIR}/vtable_gen.cpp)
add_executable(vtable_impl ${CMAKE_SOURCE_DIR}/vtable_impl.cpp)

install(TARGETS vtable_gen vtable_impl DESTINATION bin)
