project(Tinyhttpd)

cmake_minimum_required(VERSION 3.0.0)

add_executable(httpd httpd.cpp)

# find_package(pthread REQUIRED)
target_link_libraries(httpd pthread)