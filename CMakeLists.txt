cmake_minimum_required(VERSION 3.25)
project(flappy_bird CXX)

find_package(SDL2 REQUIRED)

add_executable(${PROJECT_NAME} WIN32 src/main.cpp)
target_link_libraries(${PROJECT_NAME} PRIVATE SDL2::SDL2main SDL2::SDL2-static)
