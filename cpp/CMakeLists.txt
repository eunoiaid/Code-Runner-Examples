cmake_minimum_required(VERSION 3.13)
project(hello LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

add_executable(main ${CMAKE_CURRENT_LIST_DIR}/src/main.cpp ${CMAKE_CURRENT_LIST_DIR}/src/greeting.cpp)
target_include_directories(main PRIVATE ${CMAKE_CURRENT_LIST_DIR}/include)