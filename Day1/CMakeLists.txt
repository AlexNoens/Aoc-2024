cmake_minimum_required(VERSION 3.20)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_CXX_COMPILER "g++")
set(CMAKE_C_COMPILER "gcc")
set(LIB_PATH "../lib")

project(Day1)

add_subdirectory(solver)
add_subdirectory(${LIB_PATH} "${CMAKE_BINARY_DIR}/lib")

add_executable(Day1 main.cpp)

target_link_libraries(Day1 PUBLIC solver puzzleFetcher)
target_include_directories(Day1 PRIVATE ${LIB_PATH})
