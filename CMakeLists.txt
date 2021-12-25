cmake_minimum_required(VERSION 3.10)
project(OS_HW3)

set(CMAKE_CXX_STANDARD 11)

add_executable(OS_HW3_SERVER server.c segel.c request.c)
add_executable(OS_HW3_CLIENT client.c segel.c)