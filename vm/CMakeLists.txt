cmake_minimum_required(VERSION 3.8)

SET (CMAKE_CXX_STANDARD 11)
SET (CMAKE_CXX_STANDARD_REQUIRED ON)

project("vm" C)

SET(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -static")

add_executable(${PROJECT_NAME}
    "vm.c"
    "vm_dbg.c"
    "vm_dbg.h"
)