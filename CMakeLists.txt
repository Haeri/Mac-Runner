cmake_minimum_required(VERSION 3.3)

set(PROJECT_NAME moltenvk_vcpkg_test)
project(${PROJECT_NAME} LANGUAGES CXX)

file(GLOB SOURCE_FILES main.cpp)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})