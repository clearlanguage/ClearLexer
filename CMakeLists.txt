cmake_minimum_required(VERSION 3.29)
include(FetchContent)
project(ClearLexer)

set(CMAKE_CXX_STANDARD 20)


FetchContent_Declare(
        fast_float
        GIT_REPOSITORY https://github.com/fastfloat/fast_float.git
        GIT_TAG tags/v6.1.6
        GIT_SHALLOW TRUE)

FetchContent_MakeAvailable(fast_float)


add_executable(ClearLexer Source.cpp
        Lexer.cpp)


target_link_libraries(ClearLexer PUBLIC fast_float)
