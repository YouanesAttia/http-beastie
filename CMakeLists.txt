cmake_minimum_required(VERSION 3.10)
project(server)

find_package(Boost REQUIRED)

add_executable(server ./src/main.cpp ./src/utils.cpp)

target_include_directories(server PRIVATE ${Boost_INCLUDE_DIRS})
