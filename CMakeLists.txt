cmake_minimum_required(VERSION 3.10)
project (space_warriors_game)

set(CMAKE_CXX_STANDARD 20)

find_package(SFML COMPONENTS System Window Graphics Audio Network REQUIRED)

add_executable(exec main.cpp)

target_link_libraries(exec sfml-graphics sfml-window sfml-system) # Link necessary SFML modules
