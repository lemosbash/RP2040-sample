cmake_minimum_required(VERSION 3.13)

set(PICO_SDK_FETCH_FROM_GIT on)
include(pico_sdk_import.cmake)

project(hello_world C CXX)

pico_sdk_init()

#standalone sanity check 
add_executable(hello_world
	src/hello_world.c
)

target_link_libraries(hello_world pico_stdlib)
pico_add_extra_outputs(hello_world)
