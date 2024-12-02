cmake_minimum_required(VERSION 3.30)
project(MIPGenerator)

set(CMAKE_CXX_STANDARD 20)

find_package(TIFF REQUIRED)

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME} PRIVATE TIFF::TIFF)
