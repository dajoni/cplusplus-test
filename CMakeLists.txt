cmake_minimum_required(VERSION 3.14)
project(cplusplus)
add_compile_options(-Wall -Wextra -pedantic -Werror)

set(CMAKE_CXX_STANDARD 14)

add_library(calcLib src/Calculator.cpp src/Modulator.cpp)

add_executable(main main.cpp)
target_link_libraries(main calcLib)
