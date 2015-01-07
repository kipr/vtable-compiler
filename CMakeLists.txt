cmake_minimum_required(VERSION 2.8.0)

project(vtable)

add_executable(vtable_gen ${CMAKE_SOURCE_DIR}/vtable_gen.cpp)
add_executable(vtable_impl ${CMAKE_SOURCE_DIR}/vtable_impl.cpp)

install(FILES ${CMAKE_BINARY_DIR}/vtable_gen ${CMAKE_BINARY_DIR}/vtable_impl DESTINATION bin)