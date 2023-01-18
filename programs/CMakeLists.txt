cmake_minimum_required(VERSION 3.8)

SET (CMAKE_CXX_STANDARD 11)
SET (CMAKE_CXX_STANDARD_REQUIRED ON)

project("programs" C)

SET(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -static")

add_executable("simple_program"
    "simple_program.c"
)

add_executable("sum_program"
    "sum_program.c"
)