cmake_minimum_required(VERSION 3.15)

cmake_policy(SET CMP0091 NEW)
cmake_policy(SET CMP0077 NEW)

project(relativity-scalar-field LANGUAGES CXX C)

set(CMAKE_CXX_STANDARD 17)

set(CMAKE_MSVC_RUNTIME_LIBRARY MultiThreaded$<$<CONFIG:Debug>:Debug>)

set(SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)

add_executable(relativity-scalar-field)

target_sources(relativity-scalar-field PRIVATE ${SOURCE_DIR}/main.cpp)