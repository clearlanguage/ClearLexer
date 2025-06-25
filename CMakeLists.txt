cmake_minimum_required(VERSION 3.28)
project(playground)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(playground Source.cpp Lexer.cpp)