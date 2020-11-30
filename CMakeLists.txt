project(Tinyhttpd)

cmake_minimum_required(VERSION 3.0.0)

add_executable(httpd httpd.cpp)

target_link_libraries(Tinyhttpd ${CMAKE_THREAD})