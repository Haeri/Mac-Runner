cmake_minimum_required(VERSION 3.3)

set(PROJECT_NAME moltenvk_vcpkg_test)
project(${PROJECT_NAME} LANGUAGES CXX)

file(GLOB SOURCE_FILES main.cpp)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})

# ---------------- DEPENDENCIES ---------------------#

# glfw3
find_package(glfw3 CONFIG REQUIRED)
target_link_libraries(${PROJECT_NAME} PRIVATE glfw)