cmake_minimum_required(VERSION 3.13)

include($ENV{PICO_SDK_PATH}/pico_sdk_init.cmake)

project(ms4525do_dev C CXX ASM)

pico_sdk_init()

add_executable(${CMAKE_PROJECT_NAME}
    main.c
)

pico_add_extra_outputs(${CMAKE_PROJECT_NAME})

target_link_libraries(${CMAKE_PROJECT_NAME} pico_stdlib)