cmake_minimum_required(VERSION 3.15)
project(test_package LANGUAGES C)

find_package(minimp3 REQUIRED CONFIG)

add_executable(${PROJECT_NAME} test_package.c)
target_link_libraries(${PROJECT_NAME} PRIVATE minimp3::minimp3)
