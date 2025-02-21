cmake_minimum_required(VERSION 3.27.8)
project(Scrolls)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

file(GLOB SCROLLS_SRC ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp)

add_library(scrolls STATIC ${SCROLLS_SRC})

target_include_directories(scrolls PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)