cmake_minimum_required(VERSION 3.10)
project(OS_HW3)

set(CMAKE_CXX_STANDARD 11)

make_directory(public)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/public/home.html DESTINATION ./public/)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/public/favicon.ico DESTINATION ./public/)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/public/output.cgi DESTINATION ./public/)

add_executable(OS_HW3_SERVER server.c segel.c request.c)
add_executable(OS_HW3_CLIENT client.c segel.c)