cmake_minimum_required(VERSION 2.8.4)

project(project_name)

#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14")
#set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/build")

set(HEADERS_PATH ${CMAKE_SOURCE_DIR}/include)

include_directories(include)

## A list of source files
set(SOURCE_FILES main.cpp)

## A list of header files here
set(HEADER_FILES )

## Add a subdirectory
#add_subdirectory(libs/yaml-cpp-0.5.1)

add_executable(${PROJECT_NAME} ${SOURCE_FILES} ${HEADER_FILES})

## Include find-pkg module 
#include(FindPkgConfig)

## Search for a lib using find-pkg
#pkg_search_module(SDL2 REQUIRED sdl2)

## Link libs
#target_link_libraries(${PROJECT_NAME})

